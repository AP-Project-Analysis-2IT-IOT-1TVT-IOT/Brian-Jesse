# Farmlab



AP Hogeschool <br>
Brian Van Campen en Jesse Denaux

## Opdrachtgever
Maarten Luyts is de productowner en begeleider van het project.

## Samenvatting

Farmlab is een project voor IOT studenten van het 2e jaar. Hierbij wordt er verder gebouwd op vorige iteraties. Er wordt verder gebouwd op iteratie vier. 

Het farmlab is een kast met 3 niveau’s waarbij planten als een hydrocultuur kunnen groeien. Dit wil zeggen dat de planten niet in de grond zitten maar met hun wortels direct in 
water liggen en via voedingsstoffen in het water kunnen groeien. Op deze manier is er geen vruchtbare grond nodig en kan de plantage in de hoogte worden uitgebereid. 

De kast wordt volledig geautomatiseerd zodat al de verschillende componenten remote kunnen worden gecontroleerd en bestuurd. 
## Situatie As-Is

![image](https://user-images.githubusercontent.com/93762886/146644024-536fc2b0-0e54-4e88-9590-6fe0a24ce765.png)

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
*Text van https://ap-it-gh.github.io/ssys21-docs-labfarm/#/README*



## Situatie To-Be

![image](https://user-images.githubusercontent.com/91600019/146584581-bf54abef-6f97-43d4-9fad-d52bca36c18a.png)

In versie vijf worden de probleemstellingen van versie vier bloot gelegd en verbeterd. Dit houdt in dat de zes verschillende componenten waaruit de kast is opgebouwd verder 
worden verfijnd en geoptimaliseerd zodat de kast een periode van één maand zelfstandig kan werken met remote besturing. Daarnaast wordt er tijdens iteratie vijf een tweede kast 
opgebouwd. 

De 3 hoofdproblemen van de as is worden verder uitgewerkt. 

<ol>
   <li>Kast</li>
    <ul>
      <li>Test 1e kast</li>
      <li>Opbouw 2e kast</li>
      <li>Temperatuur controller toevoegen</li>
    </ul>
  <li>Automatisatie</li>
    <ul>
      <li>Node Red</li>
      <li>User input</li>
      <li>Tweede pomp voor voedingsstoffen</li>
      <li>XY-systeem</li>
    </ul>
  <li>PCB's herwerken naar ESP32</li>
    <ul>
      <li>Pompcontroller</li>
      <li>Lichtsensor</li>
      <li>LED-controller</li>
      <li>Watercontroller</li>
    </ul>
</ol>


### Projectdefinitie
<ul>
  <li> Doelstelling</li>
  Het doel van iteratie 5 van het farmlab is om geen Raspberry Pi of NodeMCU's te gebruiken maar deze te vervangen door ESP32's. Daarnaast wordt er een XY systeem gebouwd met 
  een beweegbare camera en wordt er gebruik gemaakt van Node-Red. 
  <li> Scope</li>
  <ul>
    <li>AI aan XY-systeem toevoegen voor plant herkenning</li>
    <li>Temperatuur sensor toevoegen </li>
    <li>Pompcontroller systeem a.d.h.v. een ESP32</li>
    <li>Lichtsensor systeem a.d.h.v. een ESP32</li>
    <li>LED-controller systeem a.d.h.v. een ESP32</li>
    <li>Watercontroller systeem a.d.h.v. een ESP32</li>
    <li>Temperatuur sensor systeem a.d.h.v. een ESP32</li>
    <li>Opbouw van 2e kast</li>
    <li>Systeem afstelling voor basilicum</li>
    <li>Simplistische UI</li>
    <li>Automatisatie van de verschillende systemen</li>
  </ul>
  <li> Niet in scope</li>
  <ul>
     <li>Systeemspecificaties voor verschillende planten</li>
     <li>Back-up systeem voor indien de elektriciteit uitvalt</li>
     <li>pH-controller</li>
  </ul>
</ul>

## Planning (1e semester)

<ul>
  <li>Kanban</li>
  <li>Sprint per week op donderdag</li>
  <li>Tools : word , github(project kanban)</li>
</ul><br>


| Hoofdlijnen |  Datum      | Student    |
| ----------- | ----------- |----------- |
| As is / To be| 2 Dec      |Jesse|
| Functioneel design| 2 dec |Brian, Jesse|
| Technische design | 9 dec |Brian, Jesse |
| Beschrijving van mogelijke interfaces | 9 dec|TBD|
| Beschrijving van eventuele datamigratie | 9 dec |TBD|
| Beschrijving van eventuele impact op de huidige infrastructuur | 16 dec|TBD|
| Analyse van security en eventuele autorisatierollen | 16 dec|TBD|
| Uitvoering planning | 23 dec|TBD|
| Documentatie | 23 dec|TBD|
| Samenvatting| 23 dec |Jesse Denaux|
| Bronvermelding | Continue |Brian en Jesse|

### Gantt schema

![1](https://user-images.githubusercontent.com/93762886/146636244-de3198b8-4f22-4d2a-94ac-b14f2a551c3b.png)


## Planning uitvoering (2de semester)

De uitvoering begint met de aankoop van het desbetreffende materiaal. Dit gebeurd al helemaal in het begin om rekening te houden met levertijden die enige tijd kunnen duren. 
Tijdens de bestelling kunnen de verschillende sensoren en controllers al worden aangepast en geoptimaliseerd. Daarnaast kunnen de problemen van de vierde versie worden bekeken 
en opgelost indien dit al mogelijk is. 
Nadat er een sensor of controller is aangepast moet deze al direct worden getest. Op deze manier kan er, mocht er probleem optreden, een oplossing worden gezocht voor de 
specifieke sensor of controller. Er kunnen zo kleine fouten worden opgelost die tijdens het testen van de kast voor serieuze problemen kunnen zorgen. 

| Hoofdlijnen |  Datum      | Student    |
| ----------- | ----------- |----------- |
| Aankoop materiaal | 1e maand | TBD|
| Aanpassen PCB LED-controller| Helft 1e maand tot einde 2e maand  |TBD|
| Aanpassen PCB lichtsensor| Helft 1e maand tot einde 2e maand |TBD|
| Aanpassen PCB temperatuursensor| Helft 1e maand tot einde 2e maand |TBD|
| Aanpassen PCB watersensor| Helft 1e maand tot einde 2e maand |TBD|
| Checken pomp controller| 2e maand |TBD|
| XY-syteem| Helft 1e maand tot einde 2e maand  |TBD|
| Kast kabelmanagement| Helft 2e maand tot helft 3e maand |TBD|
| Kast uittesten voor een maand| Helft 3e maand tot einde  |TBD|

### Gantt schema

![2](https://user-images.githubusercontent.com/93762886/146636251-3aa08084-8e7a-4b77-851d-279c9070424b.png)

## Functioneel design

![DFD](https://user-images.githubusercontent.com/93762886/146795045-ac3a64b3-80fb-477b-823e-1c47a1c239ee.jpg)
![DFD Data dictionary](https://user-images.githubusercontent.com/93762886/146795055-6e402e86-6a38-4a36-b59b-21eeb7be4c72.jpg)

De analyse wordt uitgewerkt voor basilicum. Basilicum is een kruid dat op een relatief gemakkelijke manier in een diepwatercultuur kan worden geteeld.

De kast bestaat uit verschillende onderdelen:

<ul>
  <li>Pompcontroller</li>
      De pompcontroller moet in staat zijn om het water op het gepaste moment rond te pompen. Hierdoor kunnen er geen algen of andere planten in het water groeien doordat het
  water te lang heeft stil gestaan. Dit proces moet automatisch gebeuren zodat de gebruiker niet om de zoveel tijd manueel de pomp moet aanzetten. Daarnaast is er nog een tweede 
  pomp om de voedingsstoffen toe te voegen aan het water zodat de planten optimaal kunnen groeien. Ook deze wordt geautomatiseerd en remote aanpasbaar zodat de hoeveelheden 
  voedingstoffen kunnen worden aangepast indien nodig. Tot nu toe werd er gewerkt met een pomp die manueel werd aangestuurd en zitten ze in het proces om te kijken of al de 
  buizen waterdicht zijn. 
  Basilicum heeft verschillende voedingsstoffen nodig om te kunnen groeien. Kalium en calcium zijn twee voedingswaarden waar basilicum voldoende van moet krijgen. Deze moeten op 
  een 1:1 basis worden gegeven. Daarnaast spelen magnesium en stikstof nog een significante rol. Het magnesium gehalte zou 50 ppm moeten zijn. Aan de hand van de electric 
  conductivity (EC) kan er worden gekeken of de basilicum genoeg voedingsstoffen kan opnemen. De EC is het zoutgehalte in het voedingswater en wordt uitgedrukt in μS/cm. De EC 
  zou een waarde tussen 1.6 en 2.2 μS/cm moeten hebben. 
   <li>LED-Controller</li>
      De LED-controller moet in staat zijn om het gepaste licht te produceren voor basilicum gebasseerd op het omgevingslicht gemeten via de licht sensor. Deze moet remote 
  aanpasbaar zijn zodat, indien de 'gezondheid' van de plant achteruit gaat, de gebruiker deze kan aanpassen zonder zich naar de kast te moeten verplaatsen en dit in de code 
  moet gaan aanpassen. Per niveau is er een LED-controller zodat de LED's per niveau kunnen worden aangepast. 
  Basilicum moet een ten minste 14u-16 licht op een dag krijgen. Daarnaast moet het voor minimum 8u donker zijn. In de 14u dat de basilicum licht krijgt moet er een Daily Light 
  Intergral (DLI) van minstens 12 mol/m2 per dag worden overschreden. Met deze twee waarden kan er dan berekend worden hoeveel lux basisilicum moet krijgen en hoeveel lux de LED 
  lampen moeten geven. 
  Om van DLI naar lux te kunnen gaan moeten we eerst nog een tussenstap nemen. Dit is de Photosynthetic Photon Flux Density (PPFD). De PPFD is een waarde die aangeeft hoeveel 
  fotonenstroomdichtheid er is in het fotosynthetisch actieve lichtspectrum van het zonlicht. Dit bevindt zich tussen 400 en 700nm. De PPFD is uitgedrukt in µmol fotonen/m²s. Om 
  zeker te zijn dat de basilicum voor voldoende tijd genoeg licht heeft gekregen gaan we in onze berekeningen rekenen dat de basilicum voor 15u licht krijgt. We weten dat 
  basilicum een PPFD moet hebben tussen de 150 en 300 µmol fotonen/m²s. Bij een PPFD van 225 µmol fotonen/m²s voor 15u verkrijgen we een DLI van 12.15 mol/m2. Omdat dit dicht 
  tegen de minimum grens van onze 12 mol/m2 DLI is beslissen we om voor een PPFD van 250 µmol fotonen/m²s voor 15u te gaan. Dit komt dan uit op een DLI van 13.5 mol/m2. Om gezet 
  naar lux is dit 2818 lux voor een Red + Blue LED met een golflengte van 450 + 650nm. Dit zijn allemaal theoretische waarden. Verder tests moeten uitwijzen of deze waarden ook 
  effectief ideaal zijn voor basilicum. Er kan tijdens het testen van de kast per niveau een andere waarde kunnen worden ingesteld die bereikt moet worden om zo tebekijken welke 
  waarde het meest optimaal is. 
  <li>Lichtsensor</li>
       De lichtsensor detecteert het omgevings licht en geeft dit door aan de LED-controller. De LED-controller past de licht sterkte van de LED dan aan om de gepaste lux te 
  bekomen. Indien het omgevings licht 2000 lux is zal de LED controller de LED's aansturen om de overige 818 lux, indien er gestreefd wordt om een PPFD van 250 µmol fotonen/m²s 
  te bereiken, te geven. 
  <li>XY-systeem</li>
      Het XY-systeem is het systeem dat zich aan de achterkant van de kast bevindt. Dit systeem dient om, aan de hand van een camera en AI, te herkennen wanneer de plant die in 
  de kast wordt geteeld volgroeid is en deze dan met het XY-systeem te oogsten. Daarnaast kan dit systeem informatie sturen over het groeiproces van de plant, het pomp systeem 
  aanpassen indien nodig alsook de belichting. Het XY-systeem met zijn AI is als ware de brein van het Farmlab. Momenteel is het XY-systeem op de kast gemonteerd en kan dit 
  bewegen in het XY-vlak maar is er nog geen camera of AI systeem geïnstalleerd. 
  <li>Temperatuursensor</li>
      De temperatuursensor meet de omgevingstemperatuur. Aan de hand van deze data kan er dan iets voorzien worden om de temperatuur te doen stijgen of dalen. Dit wordt 
  meegenomen in de analyse maar zal enkel toegevoegd worden indien er nog tijd over is. De ideale temperatuur om basilicum te laten groeien is tussen de 18 en 21 graden. 
  Daarnaast moet de luchtvochtigheid best rond de 65% blijven maar wel onder de 70%.
  <li>Watersensor</li>
      De water sensor bepaald of er genoeg water in de buizen is en stuurt de pompcontroller aan indien dit niet het geval is. Hierdoor is er op elk moment voldoende water 
  aanwezig in de buizen zodat de plant voldoende voeding kan opnemen. 
  <li>pH-sensor</li>
      De pH-sensor zorgt ervoor dat de pH waarde van het water optimaal blijft zodat de basilicum kan blijven groeien. Een pH-waarde tussen de 5.5 en 6.5 is ideaal voor 
  basilicum.
</ul> 

Referenties..

Deze onderdelen worden in het technisch design verder uitgepunt.


## Technisch design
### Smart Object (Hardware Analyse)
### Kast
![image](https://user-images.githubusercontent.com/91600019/144228425-952029da-4239-4ce4-bf58-538cb70fdf7a.png)
#### Kast ontwerp
![image](https://user-images.githubusercontent.com/91600019/144228812-acda100e-8fd4-431b-b07b-b1d94918728a.png)

Documentatie van ontwerp: https://ap-it-gh.github.io/ssys21-docs-labfarm/#/MDFiles/Modular/kast

#### Buis support V3
V3 is momenteel het finale design van de supports. Na het monteren van de V2's zijn er enkele problemen opgedoken tijdens het monteren van de supports en de buizen. De 
volgende 2 aanpassingen zorgen ervoor dat de montage makkelijker gaat. Zoals bij V2 wordt V3 ook verticaal geprint en is er nood aan supports.
- De verbreding van de poten aan de onderkant zorgen ervoor dat tijdens het monteren van de supports aan het hout met vijzen deze makkelijker bereikbaar zijn.
- De toevoeging van uitsparingen voor M4 moeren in het onderste gedeelte zorgen ervoor dat de moeren in de print vastgezet kunnen worden.

Documentatie naar vorige versies : https://ap-it-gh.github.io/ssys21-docs-labfarm/#/MDFiles/Hardware_analyse/3D-Ontwerpen

#### Buis support top
![image](https://user-images.githubusercontent.com/91600019/144415593-ff1d9519-1c01-4641-bc63-75d436ce7a8c.png)
#### Buis support bottom
![image](https://user-images.githubusercontent.com/91600019/144415648-35df6548-4976-4d9e-8b02-2e6f26a9a01a.png)

#### Groeibakje V4
Versie 4 is anders gebouwd dan de vorige versies en is ook de eind versie voor de groeibakjes. De afmetingen voor de basis en gaten blijven hetzelfde, alleen de opbouw is wat 
anders. Het model gaat eerste 16mm naar boven en dan pas begint deze schuin te gaan tot de bovenste offset-plane. Vandaar gaat het schuin zodat de planten hun wortels 
rechtstreeks in het water groeien. De techniek hiervoor is van een cirkel naar een vierkant die bij een schuine offset plane gemaakt is geweest een daarna loft te gebruiken om 
ze bij elkaar te verbinden. 

Documentatie naar vorige versies :https://ap-it-gh.github.io/ssys21-docs-labfarm/#/MDFiles/Hardware_analyse/3D-Ontwerpen

![image](https://user-images.githubusercontent.com/91600019/144416435-30955e32-0042-47d6-a0a0-b1ceff3f6622.png)

| Ring |  Groeibakje      | 
|-----------|-----------|
| Hoogte: 15mm| Hoogte: 90mm       |
| Breedte binneste diameter: 60mm| Breedte diameter1: 60mm      |
| Breedte buitenste diameter: 65mm| Breedte diameter2: 40mm      |
|| De dikte van de binnenkant: 0.5mm      |

### Opsplitsen PCB's
#### Block diagram 
![image](https://user-images.githubusercontent.com/91600019/146584658-a570a248-4655-4b34-bf59-665a1ab68321.png)
#### Hardware keuze
| Naam        |Voltage(v)   |Stroom(A)   |
| ----------- | ----------- |----------- |
| Pomp|5|0,9-1,7|
| ESP32|3,3|240m|
| Stepper Motor driver|12-24|2,5(MAX)|
| LED strip|12|400m|

#### Communicatie keuze
| Type        |Voordelen   |Nadelen   |
| ----------- | ----------- |----------- |
| Wifi|-groot bereik<br>-makkelijk uitbreidbaar<br>-middelmatige afstand<br>-snel<br>-security instelbaar<br>-connectie naar Raspberry pi server mogelijk |-verbruikt relatief veel energie|
|Bluetooth|-makkelijk<br>-relatief zuinig|-korte afstand<br>-traag<br>-geen security<br>-ondersteund weinig apparaten (max 8)|
|Bedraad |-makkelijk op korte afstand<br>-minder kans op externe verstoringen<br>-geen antenne nodig|-niet ideaal voor lange afstand (onoverzichtelijk)<br>-moeilijk uitbreidbaar|

**De keuze:**

- Bedrade communicatie gaat enkel voor zeer korte afstanden worden gebruikt of indien er geen ander optie is.
- Draadloze communicatie gaat er voor het grootste deel van het project gebruikt worden. Het geeft de meeste uitbreidmogelijkheden en zorgt dat alles overzichtelijk blijft.
Verder wordt er nog voor WIFI gekozen. Deze biedt de meest betrouwbare communicatie voor meer dan 12 devices. Aangezien we volgens een main controller / node systeem willen 
werken is dit essentieel.

#### Voeding keuze

| Type        |Voordelen   |Nadelen   |
| ----------- | ----------- |----------- |
| Batterij |-draadloos/ordelijk |-moeten opgeladen worden|
| Bedrade voeding | -makkelijk |-meer bekabeling in de kast|

**De keuze:**

Er wordt voor 'the best of both worlds' gegaan. Dit houdt in dat elke controller zo draadloos mogelijk wordt gebouwd, dus met behulp van batterijen. Er wordt wel steeds een 
backup aansluiting voor bekabelde voeding voorzien.

#### Baterij keuze


| Type        |Voltage|Max stroom|Voordelen   |Nadelen   |
| ----------- | ----------- |----------- |----------- |----------- |
| 18650 | 4,2 |4 |-makkelijk<br>-hoge stroom|groot - moet in houder|
| Lithium Ion batterij (PRT-13854 ROHS) | 3,7 |2,5|-klein/plat<br>-geen houder nodig<br>-voltage dicht bij ESP input voltage|- minder capaciteit|

**De keuze:**

Aangezien er voor de sensor geen grote capaciteit of vermogen nodig is, wordt er gekozen voor de Lithium Ion batterij. Deze zouden ook zonder houder kunnen worden bevestigd aan 
de PCB. De 18650 batterijen daarentegen nemen onnodig veel plek in.

https://ap-it-gh.github.io/ssys21-docs-labfarm/#/MDFiles/Hardware_analyse/algemeen
### Analyse LED-controller

#### Block diagram

![Blokdiagram LEDController](https://user-images.githubusercontent.com/93762886/146789989-b789e21c-0e1a-409e-8a06-b4f92fecd776.jpg)


#### Schema

#### Analyse Lichtsensor controller


#### Block diagram


![Blokdiagram LightSensorController](https://user-images.githubusercontent.com/93762886/146790009-a216257d-a8ad-4b86-aeea-4f95ca419127.jpg)


### Component keuze

| naam        |Min dynamic range (Lux)|Max dynamic range (Lux)|Voeding   |Interface 	   |Prijs|
| ----------- | ----------- |----------- |----------- |----------- |----------- |
|[lichtweerstand](https://www.kiwi-electronics.nl/nl/lichtgevoelige-weerstand-ldr-416)| 1 |10|1V-200V| Analoog | 1,95€ |
| [TSL2561](https://www.adafruit.com/product/439) | 0.1 |40000 | 2,7-3,6V | I2C  	|+-5€ |
| [TSL2591](https://shop.mchobby.be/en/environnemental-press-temp-hum-gas/1599-tsl2591-sensor-lux-luminosite-lumiere-digital-3232100015999-adafruit.html) | 188µ | 	88000 |3,3-5V | I2C |  	8,69€ |
|[TSL2591](https://www.kiwi-electronics.nl/nl/si1145-digital-uv-index-ir-visible-light-sensor-1574) | NaN | NaN | 3-5V | I2C | 11,99€ |


De 'TSL2561' geeft ons de nodige accuraatheid voor een schappelijke prijs.

### Schema

### Analyse Pompcontroller

### Block diagram

![Blokdiagram PompController](https://user-images.githubusercontent.com/93762886/146790059-dca868f2-64c2-4d14-9224-255ea357c7b7.jpg)


### Schema

### Analyse Temperatuursensor

### Block diagram

![Blokdiagram TemperatuurSensor](https://user-images.githubusercontent.com/93762886/146790080-e2834bc2-4e09-4845-8594-9444ccc9da03.jpg)

### Component keuze


| naam |min temp (°C)|max temp (°C)|accuraatheid (°C)|min voltage (V)| min voltage (V) |mounting|soort|Prijs|
| ----------- | ----------- | ----------- | ----------- | ----------- | ----------- | ----------- | ----------- | ----------- |
| dht11 | 0 | 50 | 2 | 3 | 5 | thru hole | packet | 2,45 |
| dht22 | -4 | 80 | 0.5 | 3 | 5 | thru hole | packet | 9,95 |
| HIH8121-021-001 | -25 | 85 | 0.5 | 2.3 | 5.5 | SMD | apart | 7,78 |
| HIH6130-021-001 | -40 | 125 | 0.5 | 2.3 | 5.5 | thru hole | apart | 8,41 |
| SHT31-DIS-B | -40 | 125 | 0.2 | 2.15 | 5.5 | SMD reflow | apart | 4,5 |



De 'HIH6130-021-001' temperatuur en vochtigheidssensor voldoet aan onze belangrijkste eisen. Voldoende range van meetbare temperaturen en minder dan 1°C accuraatheid. Extra accuraatheid zouden we kunnen bekomen met de 'SHT31-DIS-B', deze kunnen we echter in de beginfases niet gebruiken omdat deze enkel met SMD reflow op een PCB geplaatst kan worden. Deze methode is vrij duur omdat deze stencils nodig heeft en dit niet ideaal is in de test/ontwerp fase. 

### Schema

### Analyse Watersensor

### Block diagram

![Blokdiagram WaterSensor](https://user-images.githubusercontent.com/93762886/146790117-51427c5b-35bb-4caa-bdfd-2544fd479dc4.jpg)

### Schema



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

=>MQTT omdat dit protocol gemaakt is om kleinere bytes aan data door te sturen en dit makkelijk te implementeren is in onze opstelling.

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
| Supports MQTT out of the box | Supports MQTT out of the box | Does not support MQTT out of the box (Not actively developed Plugin available) |
| Makkelijk om snel data te kunnen verwerken naar een dashboard aan de hand van flows | Eerder gemaakt voor professionele klanten, werkt met verschillende entities voor apparaten en klanten. |  |

=>Node-Red gebruiken omdat dit ingebouwde MQTT support heeft (Wat Freeboard.io niet heeft) en omdat dit op maat is van ons project (Thingsboard zou te uitgebreid zijn)




## Beschrijving van de mogelijke interfaces

Deze kast maakt gebruik van Node-RED die gaat communniceren met een ESP32 vanuit deze stuurt de gebruiker meerdere ESP32’s aan
![image](https://user-images.githubusercontent.com/91600019/146913436-9cd7562f-4817-4814-a30e-195f017d2579.png)
### Node-RED editor

![image](https://user-images.githubusercontent.com/91600019/146913720-16b7405d-04fb-4f1d-abab-c27d51c1804f.png)


### WIREFRAME
![image](https://user-images.githubusercontent.com/91600019/146914556-dccccbfb-ca62-4837-adf1-a2d299452fa5.png)
### UI
![image](https://user-images.githubusercontent.com/91600019/146913785-c37c27c9-7c5a-4eb9-8020-5b3c3a8c6749.png)



## Beschrijving van eventuele datamigratie
## Beschrijving van eventuele impact op de huidige infrastructuur
## Analyse van security en eventuele autorisatierollen
## Documentatie
## Bronvermelding
