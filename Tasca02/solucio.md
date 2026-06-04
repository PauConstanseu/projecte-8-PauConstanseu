# 🌱 Pla de Sostenibilitat Integral – Coworking Mataró

* **Autors:** Pol Serrano, Pau Constanseu i Blai Vergés.
* **Data:** 18/05/2026.
* **Consultors:** Departament de Sostenibilitat (en pràctiques).
* **Objectiu:** Transformar la infraestructura cap un model circular, reduint un 20% la factura elèctrica i obtenint una certificació.

---

## 📚 1. Índex

1. Índex.
2. Introducció a la tasca.
3. Fase 1: Diagnòstic i Auditoria.
4. Fase 2: Solucions – Hardware Circular.
5. Fase 3: Guia de Bones Pràctiques Digitals.
6. Fase 4: Pla de Sostenibilitat Integral.
7. Conclusió de la tasca.

---

## 📖 2. Introducció a la tasca

En aquesta tasca s’ha elaborat un pla de sostenibilitat per a l’empresa fictícia **Coworking Mataró**, amb l’objectiu de millorar la seva infraestructura informàtica aplicant criteris d’economia circular i eficiència energètica.

S’ha analitzat l’estat dels equips actuals, identificant problemes de consum, obsolescència i gestió de residus, i s’han proposat solucions sostenibles com l’ampliació de hardware, l’optimització energètica i la reutilització d’equips. També s’han definit bones pràctiques digitals i un pla global de sostenibilitat orientat a reduir l’impacte ambiental i millorar el rendiment dels sistemes.

---

## 👀 Fase 1: Diagnòstic i Auditoria

### Checklist d'auditoria tècnica i ambiental

| Equip | Any | Component clau | Estat tècnic | Consum estimat (W) | Punt negre identificat |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **PC 01-20** *(sobretaula)* | 2018 | HDD 500GB, 4GB DDR4, CPU Intel G5400 | Funcional però lent; sobreescalfament | 150W cadascun (en ús) | Obsolescència per manca de SSD i RAM; alta energia per tasca; residus potencials. |
| **Servidor físic** | 2017 | Xeon E5-2660, 128GB RAM, 8 HDD 1TB | Sobredimensionat per a càrrega real (només fitxers i impressió) | 500W (24/7) | Consum base altíssim; refrigeració addicional; infrautilitzat. |
| **Magatzem** | Diversos | Monitors LCD/LED, cables VGA, HDMI, fontaneria | Sense inventari; alguns monitors funcionals | N/A | Residus electrònics sense gestió; pèrdua d'oportunitat de reutilització. |

### Punts importants a destacar:
* **Consum energètic ineficient:** Els PCs amb HDD i el servidor sempre encès provoquen una factura elèctrica massa elevada.
* **Residus potencials:** El magatzem es troba desordenat i sense cap mena de classificació.
* **Obsolescència funcional:** La manca de memòria RAM i l'ús de discs lents provoca una renovació anticipada i innecessària de l'equipament.
* **Manca de pràctiques digitals:** No s'apliquen polítiques d'apagat nocturn ni de gestió eficient de dades.

---

## 💻 Fase 2: Solucions – Hardware Circular

### Catàleg de hardware recomanat (revitalització, no substitució)

| Component original | Problema | Solució circular | Producte recomanat | Millora vida útil i estalvi |
| :--- | :--- | :--- | :--- | :--- |
| **HDD 500GB** | Lent, alt consum, propens a falles. | Substituir per SSD. | SSD Kingston A400 480GB *(Energy Star)* | Redueix el temps d'accés un 80% i el consum un 70% (2W vs 6W). Allarga la vida útil del PC de 3 a 5 anys. |
| **RAM 4GB** | Insuficient per a múltiples finestres. | Ampliar a 8GB o 16GB. | Mòdul DDR4 8GB *(certificat EPEAT Gold)* | Evita el *swapping* a disc i redueix el sobreescalfament. Reutilització de sockets existents. |
| **CPU amb sobreescalfament** | Pasta tèrmica seca. | Manteniment (no substitució). | Pasta tèrmica Arctic MX-4 | Neteja i repaste. Evita la substitució prematura del processador. |
| **Servidor físic** | Sobredimensionat 24/7. | Virtualització + migració a núvul lleuger. | Servidor en mode "sleep" o Raspberry Pi per a serveis crítics. | Redueix el consum de 500W a només 15W. Allarga la vida útil de l'equip com a servidor de còpies setmanals. |
| **Monitors magatzem** | Sense ús. | Reutilització interna + donació. | Inventari i prova de funcionament. | 15 monitors funcionals es reassignaran a escriptoris compartits; reducció radical de compres noves. |

> ⚠️ **Política de compra:** Tots els nous components hauran de tenir certificació ambiental. Es prioritzaran de manera estricta els proveïdors de recanvis (ex: *second-hand* RAM/SSD certificats).

---

## 🎟️ Fase 3: Guia de Bones Pràctiques Digitals

![Fase3](/Tasca02/img/sostenibilitat.png)

---

## ♻️ Fase 4: Pla de Sostenibilitat Integral

### 1. Full de ruta de millora

| Termini | Acció | Responsable | Recursos | Indicador d'èxit |
| :--- | :--- | :--- | :--- | :--- |
| **0-3 mesos** | Auditoria de magatzem i classificació RAEE. | Tècnic IT | 10 hores | 100% d'equips inventariats. |
| | Substitució HDD -> SSD + ampliació RAM en 20 PCs. | Consultor extern | 1500 € | Temps d'arrencada < 30 segons. |
| | Implementació de política d'apagat automàtic. | Sysadmin | Configuració GPO | Consum nocturn reduït un 50%. |
| **3-6 mesos** | Virtualització del servidor (migració a serveis cloud lleugers: Nextcloud, DNS local). | Proveïdor cloud | 200 €/mes | El PUE del servidor baixa de 2.0 a 1.2. |
| | Instal·lació de monitors reutilitzats (15 unitats). | Equip coworking | 0 € (reutilització) | 0 compres noves de monitors. |
| **6-12 mesos** | Obtenció de certificació Green IT o LEED Zero Carbon. | Consultoria externa | 3000 € | Aconseguir el segell abans del mes 12. |
| | Formació trimestral als usuaris en bones pràctiques. | Responsable sostenibilitat | Intern | Participació mínima del 80% dels usuaris. |

### 2. Protocol de gestió de residus (RAEE)

* **Objectiu:** Complir amb el Reial Decret 110/2015 sobre RAEE i maximitzar la reutilització de components.
* **Procediment:**
  1. **Identificació:** Tots els aparells elèctrics i electrònics (ordinadors, cables, monitors) s'etiqueten clarament amb la data i el seu estat operatiu.
  2. **Jerarquia de residus:**
     * **Reutilització:** Equips funcionals -> donació a escoles o associacions locals (cal registrar obligatòriament el lliurament).
     * **Preparació per a la reutilització:** Neteja profunda i substitució de peces clau (SSD, RAM) -> venda al mercat de segona mà.
     * **Reciclatge:** Components absolutament no reparables (cables trencats, plaques amb mercuri) -> lliurament a un punt verd autoritzat (gestor RAEE: SIGRE o similar).
  3. **Documentació:** Emplenar de forma rigorosa la fitxa de traçabilitat (especificant model, data de baixa i destinació final).
* **Responsable:** Tècnic IT + coordinator del coworking.
* **Periodicitat:** Revisió trimestral del magatzem.

### 3. Càlcul de KPIs

#### a) PUE (Power Usage Effectiveness) – per al servidor i sala tècnica

PUE = (Energia total consumida per les instal·lacions) / (Energia consumida pels equips IT)

* **Situació actual:**
  * Energia total (servidor + refrigeració + convertidors) = 600W
  * Energia IT (només servidor) = 500W
  * PUE = 600 / 500 = 1.2 (acceptable, però millorable)

* **Objectiu (post-virtualització):**
  * Energia total = 200W (servidor lleuger + refrigeració passiva)
  * Energia IT = 150W
  * PUE objectiu = 200 / 150 = 1.33 (tot i que el consum absolut baixa un 66%)

#### b) Taxa de Reutilització de Hardware

Taxa = (Equips reutilitzats + Equips reparats + Components reutilitzats) / (Total d'equips donats de baixa en unitats, últims 12 mesos)

* **Situació actual:** 0% (tot es desplaça al magatzem sense cap mena de control).
* **Objectiu a 1 any:**
  * Equips de baixa = 20 PCs + 1 servidor + 30 monitors antics = 51 unitats
  * Reutilitzats internament = 15 monitors + 5 PCs revitalitzats = 20 unitats
  * Donats a entitats = 10 PCs (després de neteja) + 10 monitors = 20 unitats
  * Reciclats = 11 unitats (cables, plaques trencades)
  * Taxa de reutilització = (20 + 20) / 51 = 78.4% (excel·lent, >75% segons l'estàndard circular)

### Contribució als ODS

| ODS | Contribució del pla |
| :--- | :--- |
| **ODS 7: Energia assequible i no contaminant** | Reducció del consum elèctric global del 20% mitjançant l'ús de SSD i polítiques actives d'apagat. |
| **ODS 9: Indústria, innovació i infraestructura** | Revitalització d'equips i allargament dràstic de la seva vida útil. |
| **ODS 12: Producció i consum responsables** | Aplicació del protocol RAEE, reutilització de monitors i assoliment d'una taxa de reutilització >75%. |
| **ODS 13: Acció climàtica** | Disminució directa de les emissions de CO2 equivalents. |

### Annex – Resum executiu per a la certificació

* **Accions clau:**
  * Auditoria completada amb èxit (checklist complet).
  * Inversió en SSD/RAM de 1500 €, amb un retorn d'amortització estimat en 8 mesos gràcies a l'estalvi elèctric.
  * Protocol RAEE correctament implantat.
  * KPI de reutilització previst del 78% durant el primer any.
* **Compliment dels criteris ASG (Ambiental, Social, Governança):**
  * **Ambiental:** Reducció directa d'emissions de carboni.
  * **Social:** Donació altruista d'equips informàtics a escoles locals.
  * **Governança:** Nova política de compra verda i traçabilitat total de residus.
* **Proper pas:** Sol·licitar oficialment el segell *Green IT Bronze (The Green Grid)* abans de 6 mesos.

---

## 🎯 7. Conclusió a la tasca

Aquesta activitat ha permès entendre la importància crítica de la sostenibilitat dins del sector tecnològic, demostrant de forma pràctica que és perfectament possible millorar el rendiment dels equips i reduir costos econòmics sense haver de substituir tota la infraestructura existent.

Mitjançant l’anàlisi optimitzada dels recursos, la reutilització intel·ligent de hardware i la definició de bones pràctiques, s’ha desenvolupat una proposta altament eficient, sostenible i alineada amb les necessitats actuals de les empreses i el medi ambient.

**Gràcies per la vostra atenció!**
