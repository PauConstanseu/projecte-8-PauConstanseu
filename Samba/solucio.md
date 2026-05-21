# INFORME FINAL – UD10: Servidor de fitxers amb Samba

**Curs:** CFGM Sistemes Microinformàtics i Xarxes  
**Matèria:** 0224 Sistemes Operatius en Xarxa  
**Tema:** UD10. Samba  
**Data:** 19/05/2026  
**Alumne:** Pau Constanseu

---

## Exercici 1: Instal·lació i configuració de SAMBA

**Objectiu:** Instal·lar Samba, crear les carpetes compartides, crear usuaris i donar-los d'alta a Samba.

### Comandes executades:

```bash
sudo apt install samba -y

sudo mkdir -p /srv/samba/publica
sudo mkdir -p /srv/samba/compartida
sudo chown root:sambashare /srv/samba/publica /srv/samba/compartida
sudo chmod 770 /srv/samba/publica /srv/samba/compartida

sudo useradd -m -s /usr/sbin/nologin -G sambashare samba1
sudo useradd -m -s /usr/sbin/nologin -G sambashare samba2
sudo useradd -m -s /usr/sbin/nologin -G sambashare samba3

sudo smbpasswd -a samba1
sudo smbpasswd -a samba2
sudo smbpasswd -a samba3

sudo mv /etc/samba/smb.conf /etc/samba/smb.conf.backup
sudo touch /etc/samba/smb.conf
```

![Cap](/Samba/img/1.png)

![Cap](/Samba/img/2.png)

![Cap](/Samba/img/3.png)

![Cap](/Samba/img/4.png)

![Cap](/Samba/img/5.png)

## Exercici 2: Accés a carpeta pública en mode anònim

**Objectiu:** Compartir la carpeta publica de manera anònima i només lectura.

Configuració de /etc/samba/smb.conf:

```

[global]
   workgroup = WORKGROUP
   server string = Samba Server
   security = user
   map to guest = Bad User
   guest account = nobody
   log file = /var/log/samba/log.%m
   max log size = 1000
   server role = standalone server

[publica]
   path = /srv/samba/publica
   read only = yes
   guest ok = yes
   guest only = yes
   public = yes
   browseable = yes

```

![Cap](/Samba/img/6.png)

### Comprovació:

```
testparm
```
![Cap](/Samba/img/7.png)

### Creació d'arxius de prova:

```
sudo touch /srv/samba/publica/arxiu1.txt
sudo touch /srv/samba/publica/arxiu2.txt
echo "Hola" | sudo tee /srv/samba/publica/readme.txt

```

![Cap](/Samba/img/8.png)

## Exercici 3: Carpetes personals

**Objectiu:** Que cada usuari pugui accedir al seu directori personal amb tots els permisos.

### Configuració afegida a smb.conf:

```
[homes]
   comment = Directoris personals
   browseable = no
   writable = yes
   valid users = %S
   create mask = 0700
   directory mask = 0700

```
![Cap](/Samba/img/9.png)

## Exercici 4: Unitats compartides

Objectiu: Compartir compartida amb permisos diferenciats i bloquejar fitxers .zip.

### Configuració afegida:

```
[compartida]
   path = /srv/samba/compartida
   write list = samba1
   read list = samba2
   valid users = samba1, samba2
   browseable = yes
   read only = yes
   create mask = 0755
   directory mask = 0755

```
![Cap](/Samba/img/10.png)

## Bloqueig de .zip (Exercici 4.3):

```
   veto files = /*.zip/
   delete veto files = yes

```
![Cap](/Samba/img/11.png)

## Configuració final completa (fitxer smb.conf):

![Cap](/Samba/img/6.png)

## Exercici 5: Samba des de Windows 11 a Linux

Objectiu: Des de Linux, accedir a una carpeta compartida de Windows.

### Instal·lació del paquet a Zorin:

```
sudo apt install python3-smbc -y

```
![Cap](/Samba/img/12.png)

## Configuració a Windows 11:

S'ha compartit la carpeta CompartidaWin amb l'usuari Todos (Everyone) en mode lectura.

![Cap](/Samba/img/13.png)

## Incidències i observacions

No ha estat possible establir la connexió entre les màquines virtuals (Zorin i Windows 11) a VirtualBox. Podia fer ping entre elles al principi però després les màquines no es trobaven.

Per tant, no s'ha pogut verificar l'accés des de Windows als recursos Samba.

Tot i això, la configuració de Samba a Linux és correcta segons testparm i els serveis estan actius.

- Data: 19/05/2026
- Alumne: Pau Constanseu
