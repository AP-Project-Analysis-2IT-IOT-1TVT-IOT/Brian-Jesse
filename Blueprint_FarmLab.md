# Farmlab



AP Hogeschool<br>
Brian Van Campen en Jesse Denaux

## Opdrachtgever
Maarten Luyts is de productowner en begeleider van het project.

## Samenvatting

Farmlab is een project voor IOT studenten van het 2e jaar. Hierbij wordt er verder gebouwd op vorige iteraties. *Wij bouwen verder op iteratie vier. 

Het farmlab is een kast van 3 niveau’s waarbij planten als een hydrocultuur kunnen groeien. Dit wil zeggen dat de planten niet in de grond zitten maar met hun wortels direct in water liggen en via voedingsstoffen in het water kunnen groeien. Op deze manier is er geen vruchtbare grond nodig en kan de plantage in de hoogte worden uitgebereid. 

De kast wordt volledig geautomatiseerd zodat al de verschillende componenten remote kunnen worden gecontroleerd en bestuurd. 
## Situatie As-Is

Momenteel wordt er aan de vierde iteratie van het farmlab gewerkt. De documentatie van de vorige groepen zijn hier te vinden:

- https://github.com/jp19-lafa/Documentation/wiki
- https://ap-it-gh.github.io/lf-xy1-docs/#/ | https://ap-it-gh.github.io/lf-xy2-docs/#/
- https://ap-it-gh.github.io/ssys21-docs-labfarm/#/README

Er zijn 3 hoofdproblemen waar er momenteel wordt aan gewerkt. Deze zijn:

<ol>
  <li>Ordelijke opbouw van de kast</li>
  <ul>
    <li>Kabelmanagement opbouwen</li>
    <ul>
      <li>Kabels op lengte</li>
      <li>Kabel bescherming</li>
      <li>Juiste kabels gebruiken</li>
    </ul>
    <li>Makkelijke installatie + demontage</li>
    <ul>
      <li>Gebruik maken van klik of schuif systeem voor bevestiging</li>
    </ul>
    <li>Betere indeling opstellen</li>
    <li>3D supports herwerken</li>
    <ul>
      <li>Minder zwaar maken</li>
      <li>Iets lager maken</li>
    </ul> 
    <li> PVC opstelling voor water en planten </li>
    <ul>
      <li>Alle buizen voor het water door te laten stromen</li>
      <li>Potjes voor planten</li>
      <li>3D houder voor pomp stabiliseren</li>
    </ul
  </ul>
  </ul>
    <li>Automatisatie</li>
    <ul>
      <li>Juiste instellingen per plant </li>
      <li>Automatische aansturing van alle componenten</li>
    </ul>
  </ul>
  <li>PCB's herwerken</li>
  <ul>
    <li>Opmaat maken van de cases</li>
    <li>ESP12 integreren ipv nodeMCU</li>
    <li>Zekering toevoegen</li>
    <li>Hoeken afronden</li>
    <li>Grotere weerstand pads</li>
    <li>Silkscreen standariseren</li>
    <li>Mosfets kunnen plat leggen</li>
    <li>Betere koeling optie voorzien</li>
  </ul>
</ol>

In grote lijnen wordt versie 3 van het Farmlab gebruiksvriendelijker gemaakt en geautomatiseerd. 

*Text van https://ap-it-gh.github.io/ssys21-docs-labfarm/#/MDFiles/Probleemstelling?id=deelproblemen*<br>
*Text van https://ap-it-gh.github.io/ssys21-docs-labfarm/#/README documentatie*



## Situatie To-Be

In versie vijf worden de probleemstellingen van versie vier bloot gelegd en verder verwerkt. Dit houdt in dat de zes verschillende componenten waaruit de kast is opgebouwd verder worden verfijnd en geoptimaliseerd zodat de kast een periode van één maand zelfstandig kan werken met remote besturing. 

De 3 hoofdproblemen van de as is worden verder uitgewerkt. 

<ol>
   <li>Kast</li>
    <ul>
      <li>Test 1e kast</li>
      <li>Opbouw 2e kast</li>
    </ul>
  <li>Automatisatie</li>
    <ul>
      <li>Node Red</li>
      <li>User input</li>
      <li>Tweede pomp voor voedingsstoffen</li>
      <li>XY systeem</li>
    </ul>
  <li>PCB's herwerken naar ESP32</li>
    <ul>
      <li>Pomp Controller</li>
      <li>Light sensor</li>
      <li>Led controller</li>
      <li>Water controller</li>
      <li>Temperatuur controller</li>
    </ul>
 
</ol>


### Projectdefinitie
## Planning
- Kanban
- Sprint per week
- Elke donderdag
- Tools : word , github(project kanban)


| Hoofdlijnen |  Datum      | Student    |
| ----------- | ----------- |----------- |
| Samenvatting| 2 Dec       |Jesse Denaux|
| As is / To be| 2 Dec      |Jesse Denaux|
| Functioneel design| 2 dec |Brian Van Campen|
| Technische design | 9 dec |TBD|
| Beschrijving van mogelijke interfaces | 9 dec|TBD|
| Beschrijving van eventuele datamigratie | 9 dec |TBD|
| Beschrijving van eventuele impact op de huidige infrastructuur | 16 dec|TBD|
|Analyse van security en eventuele autorisatierollen | 16 dec|TBD|
|uitvoering planning | 23 dec|TBD|
|Documentatie | 23 dec|TBD|
|Bronvermelding | altijd|Brian en Jesse|

### Gantt schema

![image](https://user-images.githubusercontent.com/91600019/143431525-f699a711-61bb-4028-93d6-db2c1d5af95d.png)

## Planning uitvoering (2de semester)
| Hoofdlijnen |  Datum      | Student    |
| ----------- | ----------- |----------- |
| aanpassen PCB Ledcontroller| 2de semester       |TBD|
| aanpassen PCB lichtsensor| 2de semester       |TBD|
| aanpassen PCB temperatuursensor| 2de semester       |TBD|
| aanpassen PCB watersensor| 2de semester       |TBD|
| checken pomp controller| 2de semester       |TBD|
| X-Y syteem| 2de semester      |TBD|
| kast kabelmanagement| 2de semester      |TBD|
| kast uittesten voor een maand| 2de semester      |TBD|
## Functioneel design

de bedoeling van het design is om het zo lang mogelijk te gebruiken....(verder na denken)



de kast bestaat uit verschillende onderdelen


<ul>
  <li>Pomp controller</li>
      De pomp controller moet in staat zijn om het water op het gepaste moment rond te pompen zodat er geen algen of andere planten in het water groeien doordat het         water    te lang     heeft stil gestaan. Dit proces moet automatisch gebeuren zodat de gebruiken niet om de zoveel tijd manueel de pomp moet aanzetten. Tot nu         toe wordt er gewerkt met een pomp die   manueel wordt aangestuurd en zitten ze in het proces om te kijken of al de buizen waterdicht zijn. 
  <li>Led Controller</li>
      De led controller moet in staat zijn om het gepaste licht te produceren voor de specifieke plant.
  <li>Light sensor</li>
       detecteert of de leds aan of uit moeten.
  <li>X-Y systeem</li>
      Het XY systeem is het systeem dat zich aan de achterkant van de kast bevindt. Dit systeem dient om, aan de hand van een camera en AI, te herkennen wanneer de         plant die in de     kast wordt geteeld en deze dan met het XY systeem te oogsten. Daarnaast kan dit systeem informatie sturen over het groeiproces van de plant,       het pomp systeem aanpassen indien   nodig alsook de belichting. Het XY systeem met zijn AI is als ware de brein van het Farmlab. Momenteel is het XY systeem op       de kast gemonteerd en kan dit bewegen in het XY-     vlak maar is er nog geen camera of AI systeem geïnstalleerd. 
  <li>Temperatuur sensor?</li>
      bepaald de temeratuur voor de gepaste plant de gebruiker kan dan de temeratuur bekijken
  <li>Water sensor?</li>
      bepaald of er genoeg water is dit stuurt de pomp controller aan
</ul>  

Deze onderdelen wordenin het technisch design verder uitgepunt.


## Technisch design
### Smart Object (Hardware Analyse)
### kast
![image](https://user-images.githubusercontent.com/91600019/144228425-952029da-4239-4ce4-bf58-538cb70fdf7a.png)
### kast ontwerp
![image](https://user-images.githubusercontent.com/91600019/144228812-acda100e-8fd4-431b-b07b-b1d94918728a.png)

documentatie van ontwerp: https://ap-it-gh.github.io/ssys21-docs-labfarm/#/MDFiles/Modular/kast

### buis support V3
V3 is momenteel het finale design van onze supports. Na het monteren van de V2's zijn we op enkele problemen gestoten tijdens het monteren van de supports en de buizen. De volgende 2 aanpassingen zorgen ervoor dat de montage makkelijker gaat. Zoals bij V2 word V3 ook verticaal geprint en is er nood aan supports.
- De verbreding van de poten aan de onderkant zorgen ervoor dat tijdens het monteren van de supports aan het hout met vijzen deze makkelijker bereikbaar zijn.
- De toevoeging van uitsparingen voor M4 moeren in het onderste gedeelte zorgen ervoor dat de moeren in de print vastgezet kunnen worden.

documentatie naar vorige versies : https://ap-it-gh.github.io/ssys21-docs-labfarm/#/MDFiles/Hardware_analyse/3D-Ontwerpen

### buis support top
![image](https://user-images.githubusercontent.com/91600019/144415593-ff1d9519-1c01-4641-bc63-75d436ce7a8c.png)
### buis support bottom
![image](https://user-images.githubusercontent.com/91600019/144415648-35df6548-4976-4d9e-8b02-2e6f26a9a01a.png)

### Groeibakje V4
Versie 4 is anders gebouwd dan de vorige versies en is ook de eind versie voor de groeibakjes. De afmetingen voor de basis en gaten blijven hetzelfde, alleen de opbouw is wat anders. Het model gaat eerste paar 16mm naar boven en dan pas begint die schuin te gaan tot de bovenste offset-plane. Vandaar gaat het schuin zodat de planten hun wortels rechtstreeks in het water groeien. De techniek hiervoor is van een cirkel naar een vierkant die bij een schuine offset plane gemaakt is geweest een daarna loft te gebruiken om ze bij elkaar te verbinden. 

documentatie naar vorgige versies :https://ap-it-gh.github.io/ssys21-docs-labfarm/#/MDFiles/Hardware_analyse/3D-Ontwerpen

![image](https://user-images.githubusercontent.com/91600019/144416435-30955e32-0042-47d6-a0a0-b1ceff3f6622.png)

| ring |  groeibakje      | 
|-----------|-----------|
| hoogte: 8mm| hoogte: 46mm       |
| breedte binneste diameter: 60mm| breedte diameter1: 60mm      |
| breedte buitenste diameter: 65mm| breedte diameter2: 40mm      |
|| de dikte van de binnenkant: 0.5mm      |

### opsplitsen PCB's
### blokdiagram 
![image](https://user-images.githubusercontent.com/91600019/144410226-27c9dff8-ce96-48e8-9040-76fee4c9c816.png)
### Hardware keuze
| naam        |voltage(v)   |Stroom(A)   |
| ----------- | ----------- |----------- |
| Pomp|5|0,9-1,7|
| Raspbery Pi|5|600mA-1,2|
| ESP32|3,3|240mA|
| Stepper Motor driver|12-24|2,5(MAX)|
| Led strip|12|400mA|
### Comunicatie keuze
| Type        |voordelen   |nadelen   |
| ----------- | ----------- |----------- |
| Wifi|-groot bereik<br>-makkelijk uitbreidbaar<br>-middelmatige afstand<br>-snel<br>-security instelbaar<br>-connectie naar Raspberry pi server mogelijk |-verbruikt relatief veel energie|
|Bluetooth|-makkelijk<br>-relatief zuinig|-korte afstand<br>-traag<br>-geen security<br>-ondersteund weinig apparaten (max 8)|
|Bedraad |-Makkelijk op korte afstand<br>-minder kans op externe verstoringen<br>-geen antenne nodig|-niet ideaal voor lange afstand (onoverzichtelijk)<br>-moeilijk uitbreidbaar|

**onze keuze:**

- Bedrade communicatie willen we enkel voor zeer korte afstanden gebruiken of indien er geen ander optie is.
- Draadloze communicatie gaan we gebruiken voor het grootste deel van het project, het geeft ons de meeste uitbreidmogelijkheden en zorgt dat alles overzichtelijk blijft.
Verder hebben we gekozen voor WIFI. Deze biedt de meest betrouwbare communicatie voor meer dan 12 devices. Aangezien we volgens een main controller / node systeem willen werken is dit essentieel.

### voeding keuze

| Type        |voordelen   |nadelen   |
| ----------- | ----------- |----------- |
| Batterij |-draadloos/ordelijk |-moeten opgeladen worden|
| Bedrade voeding | -makkelijk |-meer bekabeling in de kast|

**onze keuze:**

We gaan voor 'the best of both worlds'. Dit houdt in dat we elke controller zo draadloos mogelijk willen bouwen, dus met behulp van batterijen. We voorzien wel steeds een backup aansluiting voor bekabelde voeding.

### baterij keuze


| Type        |Voltage|Max stroom|voordelen   |nadelen   |
| ----------- | ----------- |----------- |----------- |----------- |
| 18650 | 4,2 |4 |-makkelijk<br>-hoge stroom|groot - moet in houder|
| Lithium Ion batterij (PRT-13854 ROHS) | 3,7 |2,5|-klein/plat<br>-geen houder nodig<br>-voltage dicht bij ESP input voltage|- minder capaciteit|

**onze keuze:**

Aangezien we voor de sensor geen grote capaciteit of vermogen nodig hebben, hebben we gekozen voor de Lithium Ion batterij. Deze zouden we ook zonder houder kunnen bevestigen aan de PCB. De 18650 batterijen daarentegen nemen onnodig veel plek in.


### Analyse LEDController

### Blok diagram

### schema

### Analyse LichtSensorController

### Blok diagram

### Component keuze

De 'TSL2561' geeft ons de nodige accuraatheid voor een schappelijke prijs.

### schema

### Analyse PompController

### Blok diagram

### schema

### Analyse TemperatuurSensor

### Blok diagram

### Component keuze

De 'HIH6130-021-001' temperatuur en vochtigheidssensor voldoet aan onze belangrijkste eisen. Voldoende range van meetbare temperaturen en minder dan 1°C accuraatheid. Extra accuraatheid zouden we kunnen bekomen met de 'SHT31-DIS-B', deze kunnen we echter in de beginfases niet gebruiken omdat deze enkel met SMD reflow op een PCB geplaatst kan worden. Deze methode is vrij duur omdat deze stencils nodig heeft en dit niet ideaal is in de test/ontwerp fase. 

### schema

### Analyse WaterSensor

### Blok diagram

### schema



### Smart Object (Software Analyse)

### Data

Data wordt grotendeels verstuurd tussen de centrale RaspberryPi (broker MQTT en NodeRED) en de ESP32's aanwezig op de PCB's.
Alle data die tussen deze 2 uitgestuurd worden zullen van het type String zijn.

<ol>
  <li>PompController: </li>
  <ul>
    <li>NodeRED -> RaspberryPi broker -> ESP32 op pompcontroller:</li>
    <ul>
      <li>Topics: farm/x/pomp/water OF farm/x/pomp/nutrients</li>
      <li>String "on" => Pomp gaat aan</li>
      <li>String "off" => Pomp gaan uit</li>
    </ul>
  </ul>
  <li>LEDController:  </li>
  <ul>
    <li>NodeRED -> RaspberryPi broker -> ESP32 op LEDController:</li>
    <ul>
      <li>Topics: farm/x/licht/level/y => y = level 1,2 OF 3</li>
      <li>String "on" => LED's op level y gaat aan</li>
      <li>String "off" => LED's op level y gaat uit </li>
    </ul>
  </ul>
  <li>Lichtcontroller: </li>
  <ul>
    <li>ESP32 op LichtSensorController -> RaspberryPi broker -> NodeRED</li>
    <ul>
      <li>Topics: farm/x/pomp/water OF farm/x/pomp/nutrients</li>
      <li>Topics: farm/x/lichtsensor/level/y => y = level 1,2 OF 3</li>
      <li>r worden Strings gestuurd die het aantal lux doorgeeft dat de sensor meet</li>
    </ul>
  </ul>
</ol>

### Flowchart
  
  ![image](https://user-images.githubusercontent.com/91600019/145188599-96b2793f-83fa-45a8-893d-eea1d06fc426.png)

### Specificaties

| HTTP        |MQTT   |
| ----------- | ----------- |
| Vrij zwaar protocol: de header van een package is al groter dan 1 bericht van MQTT
(min +- 26 bytes header vs enkele bytes MQTT message) | Weinig data → meer keuzes op fysieke laag, trage links worden mogelijk |
| Software stack / Software stack / Library Library is vrij zwaar heeft een zeer kleine footprint | Lightweight → protocol last ook in kleine devices, sensors.. met weinig geheugen & cpu power. |
| Geen ingebouwde Standaard enkele QoS mogelijkheden| Standardisatie, compatibilieit → elk device kan hetzelfde protocol gebruiken → MQTT bouwt verder op de TCP/IP stack|
| | Vereenvoudiging → bij complexe configuraties (zie principe MQTT) |

=> Wij gaan gebruik maken van MQTT omdat dit protocol gemaakt is om kleinere bytes aan data door te sturen en dit makkelijk te implementeren is in onze opstelling.

### IOT Dashboard/Platform

**We hebben een platform/server nodig om:**

- Verzamelde data weer te geven
- Controle opdrachten te sturen
- Automatisatie programma's te beheren

|Node-RED|Thingsboard|Freeboard.io|
| ----------- | ----------- | ----------- |
| Open-source | Open-source+ professional(betalend) | Open-source |
| Flows | Entities |  |
| no API | API |  |
| Supports MQTT out of the box | Supports MQTT out of the box | Does not support MQTT out of the box
(Not actively developed Plugin available) |
| Makkelijk om snel data te kunnen verwerken naar een dashboard aan de hand van flows | Eerder gemaakt voor professionele klanten, werkt met verschillende entities voor apparaten en klanten. |  |

=> Wij gaan Node-Red gebruiken omdat dit ingebouwde MQTT support heeft (Wat Freeboard.io niet heeft) en omdat dit op maat is van ons project (Thingsboard zou te uitgebreid zijn)




## Beschrijving van de mogelijke interfaces
## Beschrijving van eventuele datamigratie
## Beschrijving van eventuele impact op de huidige infrastructuur
## Analyse van security en eventuele autorisatierollen
## Documentatie
## Bronvermelding
