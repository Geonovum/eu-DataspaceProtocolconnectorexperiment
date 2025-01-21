# Het Dataspace Protocol {#4CDCCFF6}

## International Data Spaces {#021221E8}

Het Dataspace Protocol is ontwikkeld door International Data Spaces Association. De International Data Spaces Association (IDSA) is op een missie om de toekomst van de wereldwijde, digitale economie te creëren met International Data Spaces (IDS), een veilig, soeverein systeem voor het delen van data waarin alle deelnemers de volledige waarde van hun data kunnen realiseren. IDS maakt het mogelijk om nieuwe "slimme diensten" en innovatieve bedrijfsprocessen in verschillende bedrijven en industrieën te laten werken, terwijl ervoor wordt gezorgd dat de zelfbepaalde controle over data gebruik (datasoevereiniteit) in handen blijft van dataproviders.
De IDSA heeft tot doel de data-gedreven economie van de toekomst te ontsluiten door de blauwdruk te bieden voor veilige, zelfbepaalde data-uitwisseling tussen partners die elkaar vertrouwen. Dit is wat wordt aangeduid als ‘dataoevereiniteit’ en het is van vitaal belang, in het licht van het feit dat gegevenstoegang en -uitwisseling snel kritieke succesfactoren worden voor zowel bedrijven, overheid en particulieren als hele economieën. Tot nu toe hebben vooral bedrijven enorme hoeveelheden waardevolle data bewaard, die ze niet op hun eigen voorwaarden konden beheren, delen of te gelde konden maken. De IDSA heeft een referentiearchitectuur en een reeks overeenkomsten gedefinieerd die kunnen worden gebruikt om data spaces te creëren die vertrouwen tussen partners en een basis voor innovatieve, nieuwe bedrijfsmodellen, producten en diensten tot stand brengen.

Om ervoor te zorgen dat de toekomstige data-economie soepel functioneert en zijn waardepropositie waarmaakt, moeten alle spelers zich houden aan een gemeenschappelijk governancekader dat de functionele, technische, operationele en juridische overeenkomsten specificeert die hun rollen en interacties binnen en tussen de verschillende delen van het ecosysteem structureren. Dit boek met regels en richtlijnen schetst dat kader [[IDS-PPRB]]. Door deze regels en richtlijnen te volgen, kunnen alle spelers samenwerken om het gedeelde doel te bereiken om de volledige waarde van de wereldwijde data-economie te ontsluiten.

IDSA is verantwoordelijk voor het bijhouden van het regelboek en voor het ondersteunen van de toepassing ervan. De IDSA organisatie helpt bij het coördineren van belangrijke processen en als algemeen bestuur een basis voor de realisatie van interne structuren en interfaces met andere partijen. Daarnaast bestaat het IDSA Open Source project, dat de software componenten ontwikkeld voor het implementeren en testen van de essentiële IDSA componenten. De implementatie van het Dataspace Protocol heeft daarmee in de afgelopen jaren een behoorlijke vlucht genomen. De belangrijke actoren en bouwstenen van een IDS data space zijn in onderstaande figuur 3 weergegeven.

<figure id="Figuur_x">
<a href="media/IDSA data space bouwstenen (zwart).png" target="_blank"><img src="media/IDSA data space bouwstenen (zwart).png" alt=""></a>
<figcaption>IDS bouwstenen voor een data space (bron: IDSA)</figcaption>
</figure>
<br/>

De dataprovider is een apparaat, dat de data van de eigenaar overdraagt via de IDS connector naar de data space. Het stelt anderen in staat om de data te gebruiken met behoud van controle over de data: het wie, hoe, wanneer, waarom en tegen welke prijs. Dat is datasoevereiniteit, de basis voor het ontsluiten van de waarde van data. Dat wordt eveneens vastgelegd in ‘usage-policies’. 

De dataconsument is een apparaat, dat de data van de eigenaar via de IDS connector opvraagt en gebruikt vanuit de data space.

IDS Connectors zijn de ‘data gateways’. De IDS connector is een speciale softwarecomponent waarmee de deelnemers gebruiksbeleid kunnen koppelen aan hun data in een data space, het gebruiksbeleid kunnen afdwingen en naadloos de herkomst van de data kunnen volgen. De IDS connector fungeert als gateway voor data en diensten en als vertrouwde omgeving voor apps en software. 

Apps worden uitgevoerd vanuit de App Store in de vertrouwde omgeving van de IDS connector. Apps voeren taken uit zoals transacties, aggregaties of analyse van de data.

IDS-connectors kunnen de beschrijving van hun data producten (en eindpunten) publiceren bij een IDS makelaar of ‘broker’. Hierdoor kunnen potentiële dataconsumenten beschikbare data producten vinden in termen van content, structuur, kwaliteit, actualiteit en andere attributen. Met hetzelfde doel, het vinden en gebruiken van de data producten, beheren vocabulaireproviders een ‘vocabulary’, die wordt gebruikt om data producten te annoteren en te beschrijven (inclusief ontologieën, referentiedatamodellen, metadata-elementen). Vocabulaireproviders leveren deze (domeinspecifieke) vocabulaires en hun verwijzingen naar het IDS-informatiemodel, dat de basis vormt voor de beschrijving van data producten.

Het clearing house biedt decentrale en controleerbare traceerbaarheid van alle transacties indien nodig. Het is de ‘verrekenkamer’. Daarnaast biedt deze faciliteit clearing- en afwikkelingsdiensten voor alle financiële en data-uitwisselingstransacties binnen de data space.

App stores bieden data-apps aan. Dit zijn toepassingen die kunnen worden geïmplementeerd in IDS Connectors om taken zoals transformatie, aggregatie of analyse van de data uit te voeren. Data-apps kunnen worden gecertificeerd door door IDS goedgekeurde certificeringsinstanties. App stores kunnen worden geleverd door IDS-leden en moeten afzonderlijk worden gecertificeerd volgens IDS-normen.

Identiteitsproviders bieden een scala aan diensten voor het maken, onderhouden, beheren en valideren van identiteitsinformatie van en voor alle IDS deelnemers en componenten. Collectief vertrouwen in de bewijsbare identiteit van alle IDS-deelnemers is noodzakelijk voor het succesvol functioneren van op IDS gebaseerde data space.

Gecertificeerd voor betrouwbaarheid. Een transparant certificeringsproces zorgt voor vertrouwen van deelnemers en componenten binnen de data space. IDS maakt betrouwbare data-uitwisseling mogelijk tussen gecertificeerde data-aanbieders en -ontvangers, op basis van onderling overeengekomen regels.

In het figuur ? van IDSA is de data aanbieder en data consument gedefinieerd als een ‘apparaat’. In werkelijkheid is het een apparaat in handen van respectievelijk een ‘data eigenaar’ en een ‘data gebruiker’. De data eigenaar bepaalt onder welke voorwaarden en restricties (‘usage policies’) zijn/haar data wordt gedeeld met de data gebruiker. Zij zijn twee belangrijke typen participanten oftewel deelnemers in de data space. De diverse ondersteunende (technologische) diensten, die nodig zijn in een data space, zoals identity providers, catalogs brokers, data connectors of de app store, worden doorgaans geleverd door dienstverleners (‘service providers’), het derde type deelnemers in een data space. Tenslotte, dient een data space bestuurd te worden. Dat is de data space beheerder of ‘data space authority’. De data space autoriteit vervult daarbij de volgende rollen [[IDS-RAM4]]:
1. Beheert de afspraken tussen alle deelnemers in de data space; 
2. Zorgt voor het beheer van het ‘deelnemersregister’ van de data space; 
3. Is geen partij in de daadwerkelijk data-uitwisseling; data aanbieders en data gebruikers wisselen onderling data uit zonder tussenkomst van de data space beheerder.  
Alle typen deelnemers in een data space vervullen daarmee een bepaalde rol (zie figuur 4).

<figure id="Figuur_x">
<a href="media/Rollen in de dataspace (figuur TNO).png" target="_blank"><img src="media/Rollen in de dataspace (figuur TNO).png" alt=""></a>
<figcaption>Typen deelnemers (en rollen) in een data space (vrij naar TNO)</figcaption>
</figure>

<br/>
In dit Dataspace Protocol experiment gaan we kennismaken met de wijze waarop een data aanbieders en data gebruikers data kunnen uitwisselen. Dat doen we in een minimale data space setting. De data space beheerder speelt ook een rol als beheerder van het deelnemersregister. Data space dienstverleners worden vooralsnog buiten beschouwing gelaten. 
<br/>
**De data connector**<br/>
De data connector is de centrale technische component voor veilige en vertrouwde data-uitwisseling. De connector verzendt data rechtstreeks naar de consument in een vertrouwde, gecertificeerde data space, zodat de oorspronkelijke data aanbieder altijd de controle over de data behoudt en de voorwaarden voor het gebruik ervan bepaalt. De data connector maakt gebruik van technologie, die data in een soort virtuele "container" plaatst, en zorgt dat deze alleen worden gebruikt zoals overeengekomen volgens de gebruiksvoorwaarden van de data aanbieder en zijn overeengekomen tussen de betrokken partijen. In de onderstaande figuur ? is de rol van  de data connector expliciet weergeven in uitwisseling van data (producten). Daarbij kan de data connector ook worden gezien als ‘container’ als een verzameling van (meta)data en functies over de diverse aspecten, die van belang zijn voor de data-transfer tussen de data aanbieder en data consument:
1.	De data connector heeft een functie bij het beheer van deelnemers identiteiten en het deelnemersregister; <br/>
2.	De data connector bevat het data aanbod in een catalogus;<br/>
3.	De data connector kan de ‘offers’ en contracten uitonderhandelen tussen aanbieder en consument op basis van de gebruiksvoorwaarden (‘policy engine’); <br/>
4.	De data connector heeft een configuratie en monitoringsfunctie; <br/>
5.	De data connector zorgt er dat de datatransfer kan plaatsvinden tussen data aanbieder en data consument. <br/>
<br/>
**Control plane en data plane**<br/>
De data connector werkt vervolgens met gestandaardiseerde protocollen en afspraken. Een relevant concept voor het gebruik van de data connector is daarbij het onderscheid tussen control plane en data plane (zie figuur 5). Het onderscheid wordt gemaakt om aan te geven dat afspraken en standaarden voor een data space betrekking hebben op de control plane.<br/>
<br/>
De control plane (controlelaag) is verantwoordelijk voor beheer en beslissingen over hoe datastromen worden verwerkt of hoe de data space functioneert. De control plane verwerkt geen echte data, maar richt zich op controle-informatie, die nodig is om de datatransfer plaats te laten vinden op een vertrouwde en souvereine wijze. Het functioneert min of meer als een soort ‘brein’ van de data space en geeft opdrachten aan de data plane voor de data transfer. Daarmee bepaalt de control plane wat er moet gebeuren en hoe het moet gebeuren (het verzorgt de voorbereiding van de datatransfer), terwijl de data plane de uitvoering verzorgt en daadwerkelijk data transporteert. De data plane is dus verantwoordelijk voor het fysieke transport van de data  tussen aanbieder en consument. De data plane voert daadwerkelijk de datatransfer (data overdracht) uit volgens de instructies van de control plane en het verwerkt en transporteert de werkelijke data  (bijvoorbeeld een videostream, datasets, bestanden). Er zijn daarvoor diverse mogelijkheden om data transfer te laten plaatsvinden, zoals via API-verzoeken, event-streams, bulkdownloads, et cetera. De data plane schrijft voor data spaces dus niet één standaard procedure voor om data transfer te laten plaatsvinden. De controle plane bij data spaces werkt (bij voorkeur) wel volgens gestandaardiseerde protocollen en afspraken (één standaard procedure).<br/>

<figure id="Figuur_x">
<a href="media/De rol van de IDS data connector in een Dataspace IDSA.png" target="_blank"><img src="media/De rol van de IDS data connector in een Dataspace IDSA.png" alt=""></a>
<figcaption>De rol van de IDS data connector in een dataspace (vrij naar IDSA)</figcaption>
</figure>

<br/>
De IDS data connector in dit experiment werkt vervolgens met gestandaardiseerde protocollen en afspraken. Dat wordt het ‘Dataspace Protocol’ (kortweg DSP) genoemd. In de volgende paragraaf wordt de werking van het Dataspace Protocol verder beschouwd.
<br/>

## Het Dataspace Protocol

Het Dataspace Protocol is een cruciale stap in de richting van een nieuwe manier van data-uitwisseling, waarbij controle, veiligheid en interoperabiliteit centraal staan. Het biedt een gestandaardiseerde manier voor organisaties om data te delen zonder dat ze hun soevereiniteit over die data verliezen [[IDS-DSP]]. Vooral in sectoren waar vertrouwelijkheid en veiligheid van groot belang zijn, zoals gezondheidszorg, productie en logistiek, biedt dit protocol grote voordelen. De implementatie van het Dataspace Protocol heeft in de afgelopen jaren een behoorlijke vlucht genomen. Het Dataspace Protocol is een technische standaard en raamwerk dat bedoeld is om veilige en soepele data-uitwisseling mogelijk te maken tussen verschillende partijen en systemen. Dit protocol speelt een cruciale rol in het opzetten van een <b>dataspace</b> — een gedeelde digitale ruimte waarin organisaties data kunnen delen op een gecontroleerde, veilige en privacy vriendelijke manier. 
<br/>
Het Dataspace Protocol is ontworpen om een aantal belangrijke uitdagingen rond data-uitwisseling op te lossen:
<ul><li><b>Interoperabiliteit</b>: Het stelt verschillende systemen in staat om op een uniforme manier gegevens uit te wisselen, onafhankelijk van de technologie of het platform dat ze gebruiken.</li>
<li><b>Data-soevereiniteit</b>: Elke data-eigenaar houdt controle over wie toegang heeft tot hun data en onder welke voorwaarden.</li>
<li><b>Privacy en veiligheid</b>: Het protocol waarborgt dat data op een veilige manier wordt gedeeld, waarbij privacyrichtlijnen worden nageleefd, zoals de AVG (GDPR).</li>
<li><b>Transparantie</b>: Deelnemers aan een data space kunnen altijd zien wie hun data gebruikt en waarvoor deze wordt gebruikt.</li>
<br/>
Het Dataspace Protocol is een reeks van afspraken, standaarden en technologieën die worden gebruikt om veilige, gecontroleerde en interoperabele datadelen tussen de deelnemers in een data space mogelijk te maken. Het is een essentieel onderdeel van Europese data spaces, zoals die gepromoot worden door initiatieven zoals de International Data Spaces, Gaia-X en het EU Data Space Support Centre. Het Dataspace Protocol is gedefinieerd als:
<br/>
“a set of specifications designed to facilitate interoperable data sharing between entities governed by usage control and based on Web technologies. These specifications define the schemas and protocols required for entities to publish data, negotiate Agreements, and access data as part of a federation of technical systems termed a Dataspace.” [[IDS-DSP]].
<br/>
<br/>
</ul>
<b>Voordelen van het Dataspace Protocol</b>
<li>Controle en soevereiniteit: Organisaties behouden de controle over hun eigen data, zelfs als ze deze delen met andere partijen;</li>
<li>Verhoogde samenwerking: Door een standaard zoals DSP kunnen organisaties makkelijker samenwerken en data delen, wat leidt tot nieuwe kansen en innovatie;</li>
<li>Veiligheid en naleving: Dankzij ingebouwde privacybescherming en security-mechanismen wordt voldaan aan de strengste normen, waaronder de Europese privacyregelgeving (AVG).</li>
</ul>
<br/>
De onderstaande figuur 6 [[DSCC-BP]] geeft een gedetailleerd overzicht van de belangrijke concepten, componenten en protocollen voor een data space, te weten ‘Identity Governance Scope’ (bovenaan), ‘Control Plane’ (midden) en ‘Data Plane’ (onderaan). Daarbinnen zijn data connectors (links en rechts) en is het data space prototol gepositioneerd (midden). De ondersteunende componenten, zoals de ‘Vocabulary Hub’ en de ‘Catalog’ zijn aan de onderzijde weergegeven. Deze twee intermediaire en ondersteunende diensten zorgen voor het gebruik van datamodellen en formaten (de ‘vocabulary hub’) en voor de publicatie en het vinden van data (de catalogus). Op rol en functies van deze laatste twee componenten gaan we hier niet verder in.

<figure id="Figuur_x">
<a href="media/DSP systeemarchitectuur.png" target="_blank"><img src="media/DSP systeemarchitectuur.png" alt=""></a>
<figcaption>De globale systeemarchitectuur van het Dataspace Prototol [[DSCC-BP]]<figcaption>
</figure>

De figuur 6 toont een systeemarchitectuur met drie hoofdlagen [[DSCC-BP]]:
1. ‘Identity governance scope’ met drie kerncomponenten:
    - Identity register voor identiteitbeheer;
    - Identity provider, die de identity management diensten levert; 
    - Identity manager, die de identiteiten en toegangsrechten beheert.
2. De control plane is de centrale laag voor beheer en coördinatie van uiteindelijk delen van de data (de datatransfer of -uitwisseling). De control plane kent eveneens enkele onderdelen met bijbehorende protocollen: 
    - Een catalog, die zorgt voor beschrijvingen (metadata) van data en diensten;
    - Policy Negotiation, die onderhandelingen over toegangs- en gebruiksvoorwaarden faciliteert;
    - Transfer Process Management, die ervoor dat voorbereidingen worden getroffen voor Beheert processen voor data-uitwisseling. Daarbij 
    - Policy Enforcement: Verantwoordelijk voor de naleving van de onderhandelde toegangs- en gebruiksvoorwaarden.
3. Data Plane(s) zorgt voor daadwerkelijke data-uitwisseling (data exchange).
<br/>

<aside class='note' title="Making the Dataspace Protocol an international standard [[IDS-DSP-S]]">
    De specificatie werkzaamheden voor het Dataspace Protocol zijn eind 2022 gestart als subwerkgroep van WG Architectuur van IDSA. De werkgroep heeft in februari 2024 de Dataspace Protocol-specificatie 2024-1 uitgebracht. Deze versie van de Dataspace Protocol-specificatie is de releasekandidaat en wordt als stabiel beschouwd. De leden van IDSA zijn in 2017 in werkgroepen en commissies begonnen met het ontwerpen van technologie voor data spaces, zodat het Dataspace Protocol in 2024 klaar zou kunnen zijn om een standaardisatieproces te starten (zie verder [[IDS-DSP-S]]). Het Dataspace-protocol op zich is vrij licht, maar het is de essentie van het werk van IDSA. Naast het DSP vormen het IDSA Reference Architecture Model [[IDS-RAM4]], [[IDSRAM5]] en het IDSA Rulebook [[IDS-PPRB]] de kern van het werk van International Data Spaces (IDS).  
    
    Eind 2023 heeft IDSA de samenwerking gezocht met de Eclipse Foundation om het Data Space Protocol richting een internationale standaard te krijgen. Daarvoor is een gezamenlijke Eclipse Dataspace Working Group (EDWG), opgericht, die het protocol in een Eclipse Dataspace Protocol Specification-project heeft ondergebracht. Dit project zorgt voor de realisatie en oprichting van de Dataspace Technology Compatibility Kit om interoperabiliteit en naleving te kunnen garanderen. Van hieruit wordt het DSP ingediend bij ISO/IEC als een internationale norm. Het normalisatieproces door het Joint Technical Committee (JTC1) is inmiddels in gang gezet.  
</aside>
<br/>

In dit experiment staat de werking en het gebruik van het data space protocol en de data connectors centraal. Voor het delen van data met de data connector worden aldus drie stadia doorlopen, waarvoor elk verschillende protocollen zijn overeengekomen. Alvorens de werking van het data space protocol connectors in meer detail toe te lichten gaan we eerst in op het informatiemodel achter het data space protocol toe. 
<br/>

## Het Dataspace informatiemodel
pm