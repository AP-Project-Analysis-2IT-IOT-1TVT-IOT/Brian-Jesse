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
  </ul>
  <li>Automatisatie</li>
  <ul>
    <li>Juiste instellingen per plant </li>
    <li>Automatische aansturing van alle componenten</li>
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

In versie vijf worden de probleemstellingen van versie vier bloot gelegd en verder verwerkt. Dit houdt in dat de vijf verschillende componenten waaruit de kast is opgebouwd verder worden verfijnd en geoptimaliseerd zodat de kast een periode van één maand zelfstandig kan werken met remote besturing. De vijf componenten zijn: 
<ul>
  <li>Pomp controller</li>
  De pomp controller moet in staat zijn om het water op het gepaste moment rond te pompen zodat er geen algen of andere planten in het water groeien doordat het water te lang     heeft stil gestaan. Dit proces moet automatisch gebeuren zodat de gebruiken niet om de zoveel tijd manueel de pomp moet aanzetten. Tot nu toe wordt er gewerkt met een pomp die   manueel wordt aangestuurd en zitten ze in het proces om te kijken of al de buizen waterdicht zijn. 
  <li>Led Controller/Light sensor</li>
  De led controller moet in staat zijn om het gepaste licht te produceren voor de specifieke plant. 
  <li>XY systeem</li>
  Het XY systeem is het systeem dat zich aan de achterkant van de kast bevindt. Dit systeem dient om, aan de hand van een camera en AI, te herkennen wanneer de plant die in de     kast wordt geteeld en deze dan met het XY systeem te oogsten. Daarnaast kan dit systeem informatie sturen over het groeiproces van de plant, het pomp systeem aanpassen indien   nodig alsook de belichting. Het XY systeem met zijn AI is als ware de brein van het Farmlab. Momenteel is het XY systeem op de kast gemonteerd en kan dit bewegen in het XY-     vlak maar is er nog geen camera of AI systeem geïnstalleerd. 
  <li>Temperatuur sensor?</li>
  <li>Water sensor?</li>
</ul>  
In detail moeten van de vijf componenten de PCB's herwerkt worden zodat deze geen ESP12's maar ESP32's zijn. Het hele systeem moet on the spot werken en aanpasbaar zijn. Het kablemanagement moet worden herbekeken en verbeterd. 
Alles wordt zo ontworpen dat dit gemakkelijk reproduceerbaar is zodat er een tweede kast kan worden gemaakt. 



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
| X-Y syteem| 2de semester      |TBD|
## Functioneel design

de bedoeling van het design is om het zo lang mogelijk te gebruiken....(verder na denken)

### kast
![image](https://user-images.githubusercontent.com/91600019/144228425-952029da-4239-4ce4-bf58-538cb70fdf7a.png)
### kast ontwerp
![image](https://user-images.githubusercontent.com/91600019/144228812-acda100e-8fd4-431b-b07b-b1d94918728a.png)

### schema
![image](https://user-images.githubusercontent.com/91600019/144229006-644931ab-e276-4dd6-99b1-0a40964e349c.png)


de kast bestaat uit verschillende onderdelen

<ol>
  <ul>
      <li>led controller</li>
      <li>lichtsensor</li>
      <li>pomp controller</li>
      <li>temperatuur sensor</li>
      <li>water sensor</li>
      <li>X-Y systeem</li>
  </ul>
</ol>

Deze onderdelen wordenin het technisch design verder uitgepunt.


## Technisch design
### Smart Object (Hardware Analyse)
### Smart Object (Software Analyse)
## Beschrijving van de mogelijke interfaces
## Beschrijving van eventuele datamigratie
## Beschrijving van eventuele impact op de huidige infrastructuur
## Analyse van security en eventuele autorisatierollen
## Documentatie
## Bronvermelding
