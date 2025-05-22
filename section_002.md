# Het Dataspace Protocol {#4CDCCFF6}

## International Data Spaces {#021221E8}

Het Dataspace Protocol is ontwikkeld door International Data Spaces Association. De International Data Spaces Association (IDSA) is op een missie om de toekomst van de wereldwijde, digitale economie te creëren met International Data Spaces (IDS), een veilig, soeverein systeem voor het delen van data waarin alle deelnemers de volledige waarde van hun data kunnen realiseren. IDS maakt het mogelijk om nieuwe "slimme diensten" en innovatieve bedrijfsprocessen in verschillende bedrijven en industrieën te laten werken, terwijl ervoor wordt gezorgd dat de zelfbepaalde controle over data gebruik (datasoevereiniteit) in handen blijft van dataproviders.
De IDSA heeft tot doel de data-gedreven economie van de toekomst te ontsluiten door de blauwdruk te bieden voor veilige, zelfbepaalde data-uitwisseling tussen partners die elkaar vertrouwen. Dit is wat wordt aangeduid als ‘dataoevereiniteit’ en het is van vitaal belang, in het licht van het feit dat gegevenstoegang en -uitwisseling snel kritieke succesfactoren worden voor zowel bedrijven, overheid en particulieren als hele economieën. Tot nu toe hebben vooral bedrijven enorme hoeveelheden waardevolle data bewaard, die ze niet op hun eigen voorwaarden konden beheren, delen of te gelde konden maken. De IDSA heeft een referentiearchitectuur en een reeks overeenkomsten gedefinieerd die kunnen worden gebruikt om data spaces te creëren die vertrouwen tussen partners en een basis voor innovatieve, nieuwe bedrijfsmodellen, producten en diensten tot stand brengen.  
<br/>
Om ervoor te zorgen dat de toekomstige data-economie soepel functioneert en zijn waardepropositie waarmaakt, moeten alle spelers zich houden aan een gemeenschappelijk governancekader dat de functionele, technische, operationele en juridische overeenkomsten specificeert die hun rollen en interacties binnen en tussen de verschillende delen van het ecosysteem structureren. Dit boek met regels en richtlijnen schetst dat kader [[IDS-PPRB]]. Door deze regels en richtlijnen te volgen, kunnen alle spelers samenwerken om het gedeelde doel te bereiken om de volledige waarde van de wereldwijde data-economie te ontsluiten.  
<br/>
IDSA is verantwoordelijk voor het bijhouden van het regelboek en voor het ondersteunen van de toepassing ervan. De IDSA organisatie helpt bij het coördineren van belangrijke processen en als algemeen bestuur een basis voor de realisatie van interne structuren en interfaces met andere partijen. Daarnaast bestaat het IDSA Open Source project, dat de software componenten ontwikkeld voor het implementeren en testen van de essentiële IDSA componenten. De implementatie van het Dataspace Protocol heeft daarmee in de afgelopen jaren een behoorlijke vlucht genomen. De belangrijke actoren en bouwstenen van een IDS data space zijn in onderstaande figuur 3 weergegeven.
<br/>

<figure id="Figuur_x">
<a href="media/IDSA data space bouwstenen (zwart).png" target="_blank"><img src="media/IDSA data space bouwstenen (zwart).png" alt=""></a>
<figcaption>IDS bouwstenen voor een data space (bron: IDSA)</figcaption>
</figure>
<br/>

De dataprovider is een apparaat, dat de data van de eigenaar overdraagt via de IDS connector naar de data space. Het stelt anderen in staat om de data te gebruiken met behoud van controle over de data: het wie, hoe, wanneer, waarom en tegen welke prijs. Dat is datasoevereiniteit, de basis voor het ontsluiten van de waarde van data. Dat wordt eveneens vastgelegd in ‘usage-policies’.  
<br/>
De dataconsument is een apparaat, dat de data van de eigenaar via de IDS connector opvraagt en gebruikt vanuit de data space.  
<br/>
IDS Connectors zijn de ‘data gateways’. De IDS connector is een speciale softwarecomponent waarmee de deelnemers gebruiksbeleid kunnen koppelen aan hun data in een data space, het gebruiksbeleid kunnen afdwingen en naadloos de herkomst van de data kunnen volgen. De IDS connector fungeert als gateway voor data en diensten en als vertrouwde omgeving voor apps en software.  
<br/>
Apps worden uitgevoerd vanuit de App Store in de vertrouwde omgeving van de IDS connector. Apps voeren taken uit zoals transacties, aggregaties of analyse van de data.  
<br/>
IDS-connectors kunnen de beschrijving van hun data producten (en eindpunten) publiceren bij een IDS makelaar of ‘broker’. Hierdoor kunnen potentiële dataconsumenten beschikbare data producten vinden in termen van content, structuur, kwaliteit, actualiteit en andere attributen. Met hetzelfde doel, het vinden en gebruiken van de data producten, beheren vocabulaireproviders een ‘vocabulary’, die wordt gebruikt om data producten te annoteren en te beschrijven (inclusief ontologieën, referentiedatamodellen, metadata-elementen). Vocabulaireproviders leveren deze (domeinspecifieke) vocabulaires en hun verwijzingen naar het IDS-informatiemodel, dat de basis vormt voor de beschrijving van data producten.  
<br/>
Het clearing house biedt decentrale en controleerbare traceerbaarheid van alle transacties indien nodig. Het is de ‘verrekenkamer’. Daarnaast biedt deze faciliteit clearing- en afwikkelingsdiensten voor alle financiële en data-uitwisselingstransacties binnen de data space.  
<br/>
App stores bieden data-apps aan. Dit zijn toepassingen die kunnen worden geïmplementeerd in IDS Connectors om taken zoals transformatie, aggregatie of analyse van de data uit te voeren. Data-apps kunnen worden gecertificeerd door door IDS goedgekeurde certificeringsinstanties. App stores kunnen worden geleverd door IDS-leden en moeten afzonderlijk worden gecertificeerd volgens IDS-normen.  
<br/>
Identiteitsproviders bieden een scala aan diensten voor het maken, onderhouden, beheren en valideren van identiteitsinformatie van en voor alle IDS deelnemers en componenten. Collectief vertrouwen in de bewijsbare identiteit van alle IDS-deelnemers is noodzakelijk voor het succesvol functioneren van op IDS gebaseerde data space.  
<br/>
Gecertificeerd voor betrouwbaarheid. Een transparant certificeringsproces zorgt voor vertrouwen van deelnemers en componenten binnen de data space. IDS maakt betrouwbare data-uitwisseling mogelijk tussen gecertificeerde data-aanbieders en -ontvangers, op basis van onderling overeengekomen regels.  
<br/>
In het figuur 3 van IDSA is de data aanbieder en data consument gedefinieerd als een ‘apparaat’. In werkelijkheid is het een apparaat in handen van respectievelijk een ‘data eigenaar’ en een ‘data gebruiker’. De data eigenaar bepaalt onder welke voorwaarden en restricties (‘usage policies’) zijn/haar data wordt gedeeld met de data gebruiker. Zij zijn twee belangrijke typen participanten oftewel deelnemers in de data space. De diverse ondersteunende (technologische) diensten, die nodig zijn in een data space, zoals identity providers, catalogs brokers, data connectors of de app store, worden doorgaans geleverd door dienstverleners (‘service providers’), het derde type deelnemers in een data space. Tenslotte, dient een data space bestuurd te worden. Dat is de data space beheerder of ‘data space authority’. De data space autoriteit vervult daarbij de volgende rollen [[IDS-RAM4]]:
<ol>
  <li>Beheert de afspraken tussen alle deelnemers in de data space;</li>
  <li>Zorgt voor het beheer van het ‘deelnemersregister’ van de data space;</li>
  <li>Is geen partij in de daadwerkelijk data-uitwisseling; data aanbieders en data gebruikers wisselen onderling data uit zonder tussenkomst van de data space beheerder.</li>
</ol>
Alle typen deelnemers in een data space vervullen daarmee een bepaalde rol (zie figuur 4).
<br/>

<figure id="Figuur_x">
<a href="media/Rollen in de dataspace (figuur TNO).png" target="_blank"><img src="media/Rollen in de dataspace (figuur TNO).png" alt=""></a>
<figcaption>Typen deelnemers (en rollen) in een data space (vrij naar TNO)</figcaption>
</figure>

<br/>
In dit Dataspace Protocol experiment gaan we kennismaken met de wijze waarop een data aanbieders en data gebruikers data kunnen uitwisselen. Dat doen we in een minimale data space setting. De data space beheerder speelt ook een rol als beheerder van het deelnemersregister. Data space dienstverleners worden vooralsnog buiten beschouwing gelaten.  
<br/>
<br/>
<b>De data connector</b>
<br/>
De data connector is de centrale technische component voor veilige en vertrouwde data-uitwisseling. De connector verzendt data rechtstreeks naar de consument in een vertrouwde, gecertificeerde data space, zodat de oorspronkelijke data aanbieder altijd de controle over de data behoudt en de voorwaarden voor het gebruik ervan bepaalt. De data connector maakt gebruik van technologie, die data in een soort virtuele "container" plaatst, en zorgt dat deze alleen worden gebruikt zoals overeengekomen volgens de gebruiksvoorwaarden van de data aanbieder en zijn overeengekomen tussen de betrokken partijen. In de onderstaande figuur ? is de rol van  de data connector expliciet weergeven in uitwisseling van data (producten). Daarbij kan de data connector ook worden gezien als ‘container’ als een verzameling van (meta)data en functies over de diverse aspecten, die van belang zijn voor de data-transfer tussen de data aanbieder en data consument:
1.	De data connector heeft een functie bij het beheer van deelnemers identiteiten en het deelnemersregister;
2.	De data connector bevat het data aanbod in een catalogus;
3.	De data connector kan de ‘offers’ en contracten uitonderhandelen tussen aanbieder en consument op basis van de gebruiksvoorwaarden (‘policy engine’);
4.	De data connector heeft een configuratie en monitoringsfunctie;
5.	De data connector zorgt er dat de datatransfer kan plaatsvinden tussen data aanbieder en data consument. 
<br/>
<br/>
<b>Control plane en data plane</b>
<br/>
De data connector werkt vervolgens met gestandaardiseerde protocollen en afspraken. Een relevant concept voor het gebruik van de data connector is daarbij het onderscheid tussen control plane en data plane (zie figuur 5). Het onderscheid wordt gemaakt om aan te geven dat afspraken en standaarden voor een data space betrekking hebben op de control plane.  
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
De onderstaande figuur 6 [[DSSC-BP]] geeft een gedetailleerd overzicht van de belangrijke concepten, componenten en protocollen voor een data space, te weten ‘Identity Governance Scope’ (bovenaan), ‘Control Plane’ (midden) en ‘Data Plane’ (onderaan). Daarbinnen zijn data connectors (links en rechts) en is het data space prototol gepositioneerd (midden). De ondersteunende componenten, zoals de ‘Vocabulary Hub’ en de ‘Catalog’ zijn aan de onderzijde weergegeven. Deze twee intermediaire en ondersteunende diensten zorgen voor het gebruik van datamodellen en formaten (de ‘vocabulary hub’) en voor de publicatie en het vinden van data (de catalogus). Op rol en functies van deze laatste twee componenten gaan we hier niet verder in.

<figure id="Figuur_x">
<a href="media/DSP systeemarchitectuur.png" target="_blank"><img src="media/DSP systeemarchitectuur.png" alt=""></a>
<figcaption>De globale systeemarchitectuur van het Dataspace Prototol [[DSSC-BP]]<figcaption>
</figure>

De figuur 6 toont een systeemarchitectuur met drie hoofdlagen [[DSSC-BP]]:
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

<aside class='note' title="Making the Dataspace Protocol an international standard">
De specificatie werkzaamheden voor het Dataspace Protocol zijn eind 2022 gestart als subwerkgroep van WG Architectuur van IDSA [[IDS-DSP-S]]. De werkgroep heeft in februari 2024 de Dataspace Protocol-specificatie 2024-1 uitgebracht. Deze versie van de Dataspace Protocol-specificatie is de releasekandidaat en wordt als stabiel beschouwd. De leden van IDSA zijn in 2017 in werkgroepen en commissies begonnen met het ontwerpen van technologie voor data spaces, zodat het Dataspace Protocol in 2024 klaar zou kunnen zijn om een standaardisatieproces te starten (zie verder [[IDS-DSP-S]]). Het Dataspace-protocol op zich is vrij licht, maar het is de essentie van het werk van IDSA. Naast het DSP vormen het IDSA Reference Architecture Model [[IDS-RAM4]] en het IDSA Rulebook [[IDS-PPRB]] de kern van het werk van International Data Spaces (IDS).
<br/>
Eind 2023 heeft IDSA de samenwerking gezocht met de Eclipse Foundation om het Data Space Protocol richting een internationale standaard te krijgen. Daarvoor is een gezamenlijke Eclipse Dataspace Working Group (EDWG), opgericht, die het protocol in een Eclipse Dataspace Protocol Specification-project heeft ondergebracht. Dit project zorgt voor de realisatie en oprichting van de Dataspace Technology Compatibility Kit om interoperabiliteit en naleving te kunnen garanderen. Van hieruit wordt het DSP ingediend bij ISO/IEC als een internationale norm. Het normalisatieproces door het Joint Technical Committee (JTC1) is inmiddels in gang gezet.  
</aside>

<br/>

In dit experiment staat de werking en het gebruik van het Dataspace Protocol en de data connectors centraal. Voor het delen van data met een data connector worden aldus drie stadia doorlopen, waarvoor elk verschillende protocollen zijn overeengekomen. Alvorens de werking van het data space protocol connectors in meer detail toe te lichten gaan we eerst in op het informatiemodel achter het data space protocol toe. 
<br/>

## Het DSP informatiemodel

Het Dataspace Protocol vormt de basis voor interacties voor uiteindelijke vertrouwde data-uitwisseling tussen deelnemers binnen een dataspace. Om het Dataspace Protocol beter te begrijpen is inzicht in het onderliggende informatiemodel nodig. Het informatiemodel beschrijft de verschillende entiteiten, hun relaties en functies, waarbij sommige aspecten normatief zijn en andere meer abstracte concepten ter verduidelijking dienen.

Het informatiemodel benadrukt dat niet alle entiteiten een technische representatie hebben binnen de protocollen ([[IDS-IM]]). Sommige onderdelen, zoals de Participant Agent, bestaan enkel als concept en zijn niet direct zichtbaar in de communicatie tussen systemen. Het informatiemodel maakt daarbij gebruik van gestandaardiseerde definities uit externe informatiestandaarden, zoals DCAT voor het beschrijven van catalogi en datasets en ODRL voor het beschrijven van gebruiksvoorwaarden. Daarbij is wel een specifieke invulling gegeven van deze informatiestandaarden om te voldoen aan de specifieke eisen van dataspaces ([[IDS-DSP]]. Het Dataspace Protocol is daarmee samengesteld uit een combinatie van gestandaardiseerde en op maat toegepaste onderdelen en spelregels. 

Figuur 7 illustreert de relaties tussen de belangrijkste entiteiten binnen het informatiemodel van het Dataspace Protocol. Centraal in het model staat de Participant Agent, een concept dat verantwoordelijk is voor het uitvoeren van acties namens een deelnemer in de dataspace. Dit kan bijvoorbeeld bestaan uit het publiceren van informatie over dataproducten in een catalogus (metadata publiceren) of het onderhandelen over een contract voor toegang tot dataproducten en datasets.

<figure id="Figuur_x">
<a href="media/DSP informatiemodel.png" target="_blank"><img src="media/DSP informatiemodel.png" alt=""></a>
<figcaption>Het Dataspace Protocol informatiemodel ([[IDS-DSP]])<figcaption>
</figure>

De Catalog Service is een type Participant Agent, dat verantwoordelijk is voor het beheren en publiceren van een DCAT Catalog. Deze catalogus bevat metadata over datasets, die beschikbaar zijn in de dataspace. De Catalog Service heeft altijd exact één DCAT Catalog onder zijn beheer.
Een DCAT Catalog kan:
1. 0 tot N DCAT Datasets bevatten, elk met informatie of metadata over de datasets;
2. 0 tot N DCAT DataServices bevatten, die de technische details bieden over hoe de datasets of data kunnen worden verkregen via API’s of services.

Elke DCAT Dataset heeft minimaal één ODRL Offer. Een ODRL Offer of aanbieding definieert de gebruiksvoorwaarden (‘usage policy’) voor de dataset. Het legt vast hoe de dataset mag worden gebruikt door de deelnemers in de dataspace. Een dataset heeft 1..N hasPolicy-kenmerken, die een ODRL Offer bevatten, die het gebruiksbeleid definieert dat is gekoppeld aan de Catalog.  ODRL Offers mogen geen expliciete doelkenmerken bevatten. Het doel van een aanbieding is de bijbehorende Dataset. Dit is in overeenstemming met de semantiek van hasPolicy, zoals gedefinieerd in het ODRL-informatiemodel, waarin wordt uitgelegd dat de dataset automatisch het doel van elke regel is. Om conflicten te voorkomen, mag het ‘kenmerk target’ niet expliciet worden ingesteld, bijvoorbeeld in het aanbod of de regels van ODRL. 

De Connector is een ander type Participant Agent, dat verantwoordelijk is voor het uitvoeren van contractonderhandelingen en datatransfer. Het is nauw verbonden met de DCAT DataService, aangezien het technische en juridische afspraken mogelijk maakt voor toegang tot de data(set). Een succesvolle contractonderhandeling resulteert in een ODRL Agreement. Deze overeenkomst definieert de overeengekomen gebruiksvoorwaarden en verwijst naar precies één DCAT Dataset. 
Daarmee staan datasets en gebruiksvoorwaarden centraal in de interacties tussen deelnemers in de dataspace. De Catalog Service publiceert datasets en maakt deze toegankelijk via catalogi. De connectors zorgen voor de feitelijke interacties en afspraken, zoals het onderhandelen over de overeenstemming om toegang te krijgen tot de dataset.

Samengevat zijn de belangrijkste relaties tussen de entiteiten in het Dataspace Protocol: 
1.	Een catalog service beheert een catalogus van datasets en services (de DCAT catalog);
2.	Een dataset heeft één of meerdere aanbiedingen (ODRL Offer) met haar gebruiksvoorwaarden;
3.	Een connector faciliteert de onderhandeling en produceert een overeenkomst conform ODRL (ODRL Agreement) tussen producent en consument, die specifiek betrekking heeft op één dataset.

## De catalog

### DCAT metadata
De catalogus in de dataspace voorziet in de vindbaarheid van datasets van de deelnemers en zijn de basis om een datatransfer een transactie te starten. In een dataspace biedt de catalogus een overzicht van alle beschikbare datasets en diensten, die in het dataspace worden aangeboden door de aanbieders. De catalogus kan volledig publiek toegankelijk of alleen voor de deelnemers in de dataspace. Het catalog protocol definieert hoe een catalogus door een consument wordt bevraagd bij een catalogusdienst met behulp van een beschrijving van de data (producten en diensten). Deze beschrijving wordt in de vorm het metadata formaat DCAT beschikbaar opgeslagen en uitgewisseld. De Data Catalog Vocabulary (DCAT) is een vocabulaire ontwikkeld door het World Wide Web Consortium (W3C) om datasets en datacatalogi te beschrijven en met elkaar te verbinden ([[vocab-dcat-3]]). De dataset metadata in een DCAT Catalog is met de DCAT standaard beschreven en vastgelegd en wordt ook gebruikt om specifieke DCAT profielen te maken (zie ook onderstaande noot). Door het beschrijven van deze  informatie-elementen wordt voldaan aan de vereisten van het beschrijven van datasets in het Dataspace Protocol. De onderstaande tabel 1 zijn de DCAT elementen opgenomen conform DCAT, die toegepast kunnen worden om het Dataspace Protocol te implementeren ([[IDS-DSP]]). 
<br>

Tabel 1 - Overzicht van Dataspace Protocol DCAT metadata elementen

<table style='width: 100%;'>
  <caption></caption>
  <colgroup>
    <col id='col1' style='width: 30.78895233655751%;'>
    <col id='col2' style='width: 69.2110476634425%;'>
  </colgroup>
  <thead valign='top'>
    <tr>
      <th align='left' style='border-top: 0pt none #000000; border-left: 0pt none #000000; border-bottom: 0pt none #000000; border-right: 0pt none #000000; background-color: #005A9C;'>
        <p id='11350A7E'>DCAT metadata element</p>
      </th>
      <th align='left' style='border-top: 0pt none #000000; border-left: 0pt none #000000; border-bottom: 0pt none #000000; border-right: 0pt none #000000; background-color: #005A9C;'>
        <p id='3AE04064'>Beschrijving</p>
      </th>
    </tr>
  </thead>
  <tbody valign='top'>
    <tr><td><p>dct:identifier (@id)</p></td><td><p>Unieke identifier van de dataset.</p></td></tr>
    <tr><td><p>dcat:contactPoint</p></td><td><p>Contactinformatie voor vragen over de dataset.</p></td></tr>
    <tr><td><p>dcat:keyword</p></td><td><p>Trefwoorden die de dataset beschrijven.</p></td></tr>
    <tr><td><p>dcat:landingPage</p></td><td><p>URL naar de landingspagina van de dataset.</p></td></tr>
    <tr><td><p>dcat:theme</p></td><td><p>Thema’s waaraan de dataset is gekoppeld.</p></td></tr>
    <tr><td><p>dcat:conformsTo</p></td><td><p>Specificaties waaraan de dataset voldoet.</p></td></tr>
    <tr><td><p>dct:creator</p></td><td><p>De maker van de dataset.</p></td></tr>
    <tr><td><p>dct:description</p></td><td><p>Beschrijving van de dataset (meerdere talen mogelijk).</p></td></tr>
    <tr><td><p>dct:identifier</p></td><td><p>Unieke identificatie voor de dataset.</p></td></tr>
    <tr><td><p>dct:isReferencedBy</p></td><td><p>URL’s of bronnen die naar deze dataset verwijzen.</p></td></tr>
    <tr><td><p>dct:issued</p></td><td><p>Datum waarop de dataset is gepubliceerd.</p></td></tr>
    <tr><td><p>dct:language</p></td><td><p>Taal of talen waarin de dataset beschikbaar is.</p></td></tr>
    <tr><td><p>dct:license</p></td><td><p>De licentie waaronder de dataset beschikbaar is.</p></td></tr>
    <tr><td><p>dct:modified</p></td><td><p>Datum van de laatste wijziging aan de dataset.</p></td></tr>
    <tr><td><p>dct:publisher</p></td><td><p>De organisatie die verantwoordelijk is voor het publiceren van de dataset.</p></td></tr>
    <tr><td><p>dct:relation</p></td><td><p>Verwijzingen naar gerelateerde datasets of bronnen.</p></td></tr>
    <tr><td><p>dct:title</p></td><td><p>Titel van de dataset.</p></td></tr>
    <tr><td><p>dct:type</p></td><td><p>Type van de dataset, bijvoorbeeld een kaart of tabel.</p></td></tr>
    <tr><td><p>odrl:hasPolicy</p></td><td><p>Toegepaste gebruiksvoorwaarden of beleidsregels.</p></td></tr>
    <tr><td><p>dcat:distribution</p></td><td><p>Verwijzingen naar distributies (verspreidingsmethoden) van de dataset.</p></td></tr>
    <tr><td><p>dcat:spatialResolutionInMeters</p></td><td><p>Resolutie (detailniveau) van de dataset in meters.</p></td></tr>
    <tr><td><p>dcat:temporalResolution</p></td><td><p>Tijdelijke frequentie van updates.</p></td></tr>
    <tr><td><p>dct:accrualPeriodicity</p></td><td><p>Frequentie van publicatie of updates van de dataset.</p></td></tr>
    <tr><td><p>dct:spatial</p></td><td><p>Het geografisch gebied dat door de dataset wordt gedekt.</p></td></tr>
    <tr><td><p>dct:temporal</p></td><td><p>Tijdspanne die door de dataset wordt gedekt.</p></td></tr>
    <tr><td><p>prov:wasGeneratedBy</p></td><td><p>Proces of gebeurtenis die de dataset heeft gegenereerd.</p></td></tr>
  </tbody>
</table>

<aside class='note' title="Data Catalog Vocabulary (DCAT)">
Het doel van DCAT is om metadata interoperabel te maken, zodat datasets gemakkelijk kunnen worden gevonden, gedeeld en hergebruikt tussen verschillende platforms en organisaties. Het biedt een gestandaardiseerde structuur voor metadata-elementen zoals titel, beschrijving, licentie, distributies, en toegangspunten.
De eerste versie werd in 2014 gepubliceerd, met een verbeterde en uitgebreidere DCAT versie 2 in 2020 en versie 3.0 . Deze versie legt een sterkere nadruk op interoperabiliteit, ondersteuning voor API's en uitbreiding naar bredere gebruikscontexten. Een DCAT-profiel is een specifieke afgeleide set regels en richtlijnen die een subset van DCAT beschrijft en aanpast aan een bepaalde context of toepassing. Profielen bouwen voort op de standaard DCAT-specificatie, maar voegen specifieke eisen of beperkingen toe die nodig zijn voor een bepaald domein, sector, of land. Profielen kunnen verplicht stellen welke metadata-elementen moeten worden gebruikt en hoe deze moeten worden toegepast. Belangrijke Europese en Nederlandse DCAT-profielen zijn:
1. DCAT-AP (Application Profile) is het Europese applicatieprofiel van DCAT, dat is ontwikkeld om interoperabiliteit tussen Europese open data-portalen te bevorderen [[DCAT-AP]]. DCAT-AP specificeert verplichte en optionele metadata-elementen, die nodig zijn om datasets en catalogi op EU-niveau uitwisselbaar te maken, zoals het Europese dataportaal;
2. DCAT-AP-NL is de Nederlandse variant van DCAT-AP, aangepast aan de Nederlandse context en specifiek gericht op de behoeften van Nederlandse organisaties en datasets [[DCAT-AP-NL]];
3. GeoDCAT is een extensie van de DCAT-standaard die is ontwikkeld om metadata van  geografische data en diensten te integreren in datacatalogi die DCAT gebruiken [[GeoDCAT-AP]]. GeoDCAT vormt ook de brug tussen de ISO 19115 metadata standaard voor geografische datasets en DCAT, zodat geografische datasets en services naadloos kunnen worden opgenomen in open data-portalen en catalogi.
<br>

**Metadata standaarden voor geografische datasets en diensten**

Het Nederlands metadata profiel op ISO 19115 voor geografie versie 2.1.0 ([[NLISO19115]])is de Nederlandse standaard die richtlijnen biedt voor het beschrijven van geografische datasets en diensten, gebaseerd op de internationale ISO 19115-norm. Het profiel is specifiek afgestemd op de Nederlandse en Europese  geo-informatie infrastructuur en is bedoeld om consistentie en interoperabiliteit te bevorderen bij het documenteren en delen van geografische informatie / geodatasets. Het beschrijft welke metadata-elementen verplicht, aanbevolen, of optioneel zijn, en hoe deze moeten worden toegepast, inclusief specifieke aanpassingen voor Nederland. Het Nederlands metadata profiel op ISO 19115 voor geografie definieert verplichte, aanbevolen en optionele metadata-elementen voor geografische datasets. Voor geografische diensten bestaat een equivalent, de Nederlands metadata profiel op ISO 19115 voor geografie. De metadata beschreven volgens het Nederlands profiel kunnen worden opgeslagen en uitgewisseld in XML en in JSON formaat. De XML-encoding is gebaseerd op het ISO 19139-schema, dat een gestructureerd formaat biedt voor interoperabele uitwisseling van metadata tussen catalogi en geografische informatiesystemen. JSON-encoding biedt een lichtere optie die beter geschikt is voor webtoepassingen en API's. Beide formaten ondersteunen gestandaardiseerde elementen die aansluiten bij het profiel.
</aside>

<br/>

### Gebruiksfuncties voor de DCAT catalog
Naast de inhoud van de catalogus, die bestaat uit de beschrijvingen van datasets en datadiensten conform DCAT, is het ook van belang om de functies van de catalogus te bezien. De gebruiksfuncties van de catalogus maken het mogelijk voor de mens en voor machines om de catalogus ook te gebruiken en te bevragen.  

Een dataproducent, die datasets wil aanbieden aan een dataspace, zal verschillende stappen uitvoeren om datasets beschikbaar te maken voor de potentiële consumenten. Op de meest simplistische manier kent de dataproducent de dataconsument vanaf het begin en geeft hij direct informatie over beschikbare datasets, de geselecteerde eindpunten en de toegangsmechanismen. 
De eerste stap in een typisch proces voor het publiceren van datasets is het op de juiste manier maken van een beschrijving van een dataset. Daarbij kan de data provider de beschrijvingen van datasets op twee wijzen publiceren: 1. publiceren in de catalog service of 2. publiceren in een centrale catalog broker van de data space. Beiden worden hieronder kort toegelicht. 
<br/>

**Publicatie van metadata in de catalog service**
<br/>
Meestal bieden data connectoren de technische manieren om dataset beschrijvingen in de catalog service te maken en te onderhouden, bijvoorbeeld door middel van geschikte GUI's. Na het bereiken van een syntactisch en semantisch correcte beschrijving, worden ze vervolgens geïmplementeerd bij de data connector van de dataprovider en zijn ze toegankelijk voor andere  data connectoren via de eindpunten. Afhankelijk van de vragende data connector kan de geretourneerde beschrijving van de dataset verschillen. De data connector kan dus verschillende dataset beschrijvingen aanbieden onder verschillende voorwaarden voor verschillende consumenten in een data space. De beschrijvingen van datasets worden in de data connector instantie opgenomen of gepubliceerd. 
Het kan zijn dat dataproducenten en -providers de gemaakte metadata willen publiceren op een centrale catalog component in een dataspace in plaats van deze alleen aan te bieden in zijn eigen data connector instantie.
<br/>

**Catalog broker**
<br/>
De centrale catalog component wordt dan een ‘catalog broker’ (een intermediaire dienst). De data provider stuurt de metadata beschrijving van de dataset naar de centrale centrale catalog. De centrale catalog is een onderdeel van een dataspace, die de publicatie van metadata voor datasets (en ook data connectoren) in de dataspace mogelijk maakt. Dataconsumenten kunnen in de centrale catalog geschikte aanbiedingen van datasets vinden zonder het bestaan of de locatie van de aanbieder te kennen. De catalog slaat de geplaatste metadata beschrijvingen op en stelt deze ook beschikbaar voor zoekopdrachten van gebruikers en andere data connectors. Potentiële dataconsumenten kunnen de opgeslagen metadata beschrijvingen doorzoeken, filteren op relevante aanbiedingen, onderhandelen met de dataprovider en de dataset aanvragen bij de data connector. 

Het is echter niet verplicht voor een data provider om datasets te publiceren bij een catalog. Ook een dataconsument wordt niet gedwongen om zijn zoekproces te starten bij een catalog, als de consument ook andere opties heeft om zijn dataset partners te vinden en te lokaliseren. Toch hebben beide de mogelijkheid om te communiceren met een centrale catalogus. Daarvoor zijn drie functies van belang:  
1.	Het registeren van metadata in de centrale catalog door de dataprovider;
2.	Het zoeken naar datasets door consument in de centrale catalog;
3.	Onderhouden en updaten van metadata en data connectors in de centrale catalog. 

<br/>

**Het registeren van metadata bij de catalog broker**
De dataprovider kan metadata beschrijvingen naar een catalog broker sturen en publiceren (zie figuur 8). De metadata beschrijving van een dataset moet op zichzelf staan en voldoen aan de specificaties van het informatiemodel. De catalog controleert vervolgens de syntactische juistheid van de aangeleverde metadata en bewaart deze in zijn lokale database. Het controleert niet de semantische correctheid of de plausibiliteit van de verstrekte informatie. Een catalog zoekt niet actief naar metadata of zoekt het niet naar updates. De catalog vertrouwt op de metadata beschrijvingen, die is aangeleverd door de dataprovider. De dataprovider is verantwoordelijk voor de metadata in de catalog en de centrale catalog kan dus niet verantwoordelijk worden gesteld voor verouderde of verkeerde informatie. 

<figure id="Figuur_x">
<a href="media/IDS Registratie van metadata bij de catalog broker.png" target="_blank"><img src="media/Registratie van metadata bij de catalog broker.png" alt=""></a>
<figcaption>Registratie van metadata bij de catalog broker [[IDS-RAM4]]<figcaption>
</figure>
<br/>

**Het zoeken naar datasets in de catalog**
Om een dataprovider te vinden, kan de dataconsument zoeken in de catalog van een centrale catalog in de dataspace (zie figuur 9). Daarvoor moet de dataconsument een geschikte centrale catalog  selecteren en de zoekmogelijkheden bepalen grafische zoekinterfaces of domeinspecifieke zoektalen. De centrale catalog retourneert vervolgens het resultaat van de zoekopdracht naar de dataconsument. Het zoekresultaat kan verschillen afhankelijk van de bevraagde data connector als gevolg van het filteren van de weergegeven data volgens het gebruiksbeleid dat is gedefinieerd door de dataprovider. 

De dataconsument moet het resultaat interpreteren om meer te weten te komen over de verschillende beschikbare datasets. Elk zoekresultaat moet informatie bevatten over elke data connector, die de gewenste datasets kan leveren, zodat de dataconsument toegang heeft tot de zelfbeschrijving van elke data connector voor meer informatie over het ontvangen van de gewenste dataset. 

<figure id="Figuur_x">
<a href="media/IDS Zoeken naar datasets in de centrale catalog.png" target="_blank"><img src="media/IDS Zoeken naar datasets in de centrale catalog.png" alt=""></a>
<figcaption>IDS Zoeken naar datasets in de centrale catalog [[IDS-RAM4]]<figcaption>
</figure>
<br/>

**Onderhouden en updaten van metadata en data connectors in de catalogus**
De dataprovider heeft er belang bij om de metadata in de catalog goed te onderhouden. Daarvoor is het mogelijk om updateverzoeken te sturen naar de catalogus. Dit kan worden gedaan door de nieuwe metadata te verzenden, die dezelfde identifier gebruikt als de eerder verzonden metadata. De catalogus werkt vervolgens de opgeslagen metadata bij. Ook een data connector heeft de mogelijkheid zijn metadata bij de catalog te updaten.

## Contract onderhandelingen

### Controle over datagebruik met ‘policies'
Een data connector bevat in feite de beschrijvende informatie over de beschikbare datasets en informatie over het gebruik ervan in de vorm van contractaanbiedingen. In een contractaanbieding wordt beschreven onder welke voorwaarden de dataprovider bereid is zijn datasets ter beschikking te stellen aan de dataconsument. Dit kan gaan van eenvoudige tot complexe toegangsbeperkingen en restricties. 

Datasets worden doorgaans alleen beschermd door toegangscontrolemechanismen. Zodra toegang tot data is verleend, kunnen data door de ontvanger of consument worden gewijzigd, gekopieerd en verspreid. ‘Usage control’ of gebruikscontrole biedt mogelijkheden om het toekomstig gebruik te beheren na het verlenen van de eerste toegang. Gebruikscontrole voorkomt misbruik van data, beschermt intellectueel eigendom, behoudt de waarde van de data en zorgt dat de dataproducent kan voldoen aan wettelijke verplichtingen met betrekking tot het gebruik van de data. 

Eerder is gesteld, dat datasoevereiniteit betekent, dat een dataproducent volledige controle heeft over de data, Gebruikscontrole is noodzakelijk om de datasoevereiniteit te handhaven. Het regelt de toegang tot en het delen van data binnen dataspaces. Het Dataspace Protocol stelt deelnemers in staat om toegangsrechten te definiëren en richtlijnen voor het delen van data in contracten vast te stellen. Het Protocol biedt de mogelijkheid om veilige en betrouwbare data delen en datasoevereiniteit te realiseren. 

Het onderdeel gebruikscontrole beperkt de toegang tot de data ingeval van voorwaarden, juridische eisen, restricties, et cetera. Gebruikscontrole voor datasets kent vele verschijningsvormen en methoden, waarvan de bekendste twee zijn ([[IDS-RAM4]]):
1.	Role-based access control (RBAC), waarbij wordt gecontroleerd of de rol van de gebruiker overeenkomt met de gevraagde rol, bijvoorbeeld alleen een beheerder of ontwikkelaar heeft toegang tot de data;
2.	Attribute-based access control (ABAC), waarbij attributen kenmerken worden gedefinieerd en wordt gecontroleerd of deze kenmerken voldoen aan de vereisten voordat toegang tot de data(set) wordt verleend. 
Toegangsbeheer op basis van attributen of kenmerken wordt ook wel op ‘policies’ (beleid) gebaseerd toegangsbeheer genoemd, omdat het toegangsrechten verleent aan gebruikers op basis van gedefinieerd beleid. Het beleid kan meerdere attributen van de data combineren, waaronder onderwerp-, tijd en/of locatiekenmerken van datasets. Het Dataspace Protocol maakt gebruik van op attributen-gebaseerde gebruikscontrole voor data. 

### ABAC als methode
Hoe evalueer je het beleid en handhaaf je het? Stel je voor dat een gebruiker toegang zoekt tot een document. Gebruiksbeheer is een uitbreiding van toegangscontrole [[IDS-PPUC]], die is ontworpen om de deelnemers te ondersteunen bij het beschermen van hun datasets. Het voert verplichtingen uit en handhaaft de ingestelde gebruiksbeperkingen nadat de toegang is verleend. De beperkingen kunnen gelaagd zijn. Het kan bijvoorbeeld zeggen: Ja, je hebt toegang, maar slechts voor drie dagen. Of ja, maar informeer de eigenaar. 
<br/>

**Hoe specificeer je gebruiksbeleid?** 
<br/>

Om het gebruiksbeleid op datasets vast te leggen is het raadzaam een beleidsspecificatie op te stellen. Beleidsspecificatie is een ander woord voor een ‘policy contract’. Wat is een ‘policy contract’. Binnen het data space protocol wordt een beleidsspecificatie beschouwd als een “als een abstracte set regels voor het gebruik van een resource” [[IDS-RAM4]] Dit contract, dat kan worden gezien als het gebruiksbeleid, is onderverdeeld in twee onderdelen: 
1.	Contract metadata, zoals de datum waarop het contact is uitgegeven; en 
2.	Regels voor gebruiksbeheer, zoals toepassingen, toestemming-, verbod- en verplichtingsverklaringen. 
De regels voor gebruiksbeheer is het deel van het contract dat van bijzonder belang is. Het definiëren van het beleid voor gebruiksbeheer is evident voor het vertrouwd en soeverein data delen. Welk soort beleid kan worden gedefinieerd? 

De Dataspace Protocol biedt sjablonen aan, ook wel beleidsklassen genoemd, die het datagebruik beperken tot specifieke voorwaarden of bepaalde verplichtingen voor of na het datagebruik. Hier zijn drie voorbeelden: 
1.	Een consument toestaan of verbieden de data te gebruiken;
2.	Beperk het datagebruik voor specifieke doeleinden (bijvoorbeeld alleen voor onderzoek); 
3.	Gebruik de data binnen een bepaalde periode en verwijder deze daarna. 
Naarmate meer gebruiksscenario's en nodig zijn, zullen ook meer sjablonen worden geïntroduceerd om gebruikers te helpen bij het definiëren van hun beleid. Een beleid voor gebruiksbeheer wordt gevormd door een of meer exemplaren van beleidsklassen of sjablonen te combineren. 

### ODRL specificaties voor beleid van datagebruik
De beleidsregels zijn ontworpen om machinaal leesbaar en interpreteerbaar te zijn, waardoor geautomatiseerde handhaving en uitwisseling, en dus ‘contract negotiation’ mogelijk is. Binnen het IDS data space protocol wordt gewerkt met de Open Digital Rights Language (ODRL) standaard van W3C [[ODRL]] voor het uitdrukken van data gebruiksbeleid. ODRL biedt een eenvoudige structuur en een uitgebreid vocabulaire voor het opstellen van data gebruiksbeleid, inclusief de mogelijkheid om termen te definiëren en profielen te maken. ODRL policies beschrijven:
•	Permissies: wat mag iemand doen?;
•	Beperkingen: wat mag juist niet?;
•	Verplichtingen: wat moet iemand doen om iets te mogen?

ODRL policies worden uitgedrukt in machine-leesbare taal zoals JSON-LD of RDF/XML (zie noot met twee voorbeelden) en zijn geschikt voor automatische afhandeling van gebruiksbeleid door dataportals, data connectoren en policy engines en registers. Met ODRL kunnen contractvoorwaarden geautomatiseerd worden afgedwongen, hetgeen essentieel is in data spaces waar veel organisaties op een gestandaardiseerde manier data delen.

<aside class='note' title="Voorbeeld ODRL code in JSON-LD">
<br>

**Voorbeeld 1: ODRL code van dataset met CCO-licentie**
<br>
Een dataset met een CC0-licentie (Creative Commons Zero) is volledig vrijgegeven voor publiek gebruik, zonder enige beperkingen. Iedereen mag deze dataset gebruiken, delen, wijzigen en verspreiden, voor elk doeleinde, zonder attributieplicht of andere beperkingen. In ODRL termen zijn alleen permissies nodig en gelden geen beperkingen of verplichtingen. Hier is een voorbeeld van een ODRL-policy voor een dataset onder een CC0-licentie, uitgedrukt in JSON-LD:

ODRL-beleid voor een CC0-gelicentieerde dataset in een machine-leesbare ODRL policy (JSON-LD). De ‘target’ is de URI van de dataset waarop deze policy van toepassing is en de ‘action’ beschrijft welke handelingen zijn toegestaan: gebruik, distributie, reproductie en aanpassing. Er zijn geen constraints, geen duties, en geen prohibitions, omdat CC0 geen beperkingen oplegt.

<figure id="Figuur_x">
<a href="media/ODRL code voorbeeld 1"><img src="media/ODRL code voorbeeld 1.png" alt=""></a>
</figure>
<br/>

**Voorbeeld 2: in JSON-LD**
In dit voorbeeld is een policy opgenomen, waarin een organisatie A data mag gebruiken voor onderzoek, maar moet wel verwijzen naar de bron en de data niet commercieel mag inzetten. 

<figure id="Figuur_x">
<a href="media/ODRL code voorbeeld 2.png" target="_blank"><img src="media/ODRL code voorbeeld 2.png" alt=""></a>
</figure>

</aside>
<br>

**Policies aanmaken en het register met beleidspecificaties**
<br>
Is het nodig om te weten hoe ODRL technisch werkt om een policy voor data te specificeren? Nee, in principe niet. Wanneer een producent of provider van plan is data aan te bieden, gebruiken ze een policy editor om een policy te specificeren, wat resulteert in een contractaanbod. In een zogenaamde beleidseditor en een bijbehorend registers worden beleidsspecificaties gemaakt en bewaard. Deze beleidsspecificaties zijn beschikbaar om producten en consumenten met verschillende achtergronden en expertises in staat te stellen om met sjablonen hun beleidsspecificaties te maken en te hergebruiken. 
<br>

**ODRL Policies in DCAT metadata**
<br>
Het opnemen van een ODRL policy verloopt via de metadata beschrijving van de data(set) in DCAT formaat. De policy metadata wordt in DCAT opgenomen een DCAT-element odrl:hasPolicy. Een policy kan op verschillende wijzen in het DCAT-element odrl:hasPolicy opgenomen worden:   
1.	Via een externe verwijzing via een URL. De URL verwijst naar een ODRL-policy, die op het web beschikbaar is als een afzonderlijk resource (bijv. een RDF-bestand). Het voordeel is de bron daardoor herbruikbaar is en is losgekoppeld van de dataset (makkelijker versiebeheer);
2.	De policy wordt direct in hetzelfde document (RDF) inline gedefinieerd als de dataset.Inline opnemen in hetzelfde RDF-document;
3.	Er wordt een verwijzing opgenomen naar een gestandaardiseerde URI voor bekende licenties, bijvoorbeeld naar een machine-leesbare versie van Creative Commons. Daarvoor dient de betreffende licentiepagina wel een ODRL RDF te bevatten;
4.	Er wordt een verwijzing naar een geregistreerd policy in een policyregister opgenomen;
5.	Er wordt verwijzing naar een API, een PID of dereferenceable URI opgenomen. Deze URI kan worden opgehaald en levert een ODRL Policy op in RDF.
DCAT en ODRL zijn aldus verbonden via dit gezamenlijke DCAT-element odrl:hasPolicy. 

### Het uitvoeren van contractonderhandelingen
Op dezelfde manier kan de gebruiker de beleidseditor gebruiken om een aanvraag te maken. Deze contractaanvragen en aanbiedingen gaan een onderhandelingsproces in, kunnen onderhandelen en een overeenkomst tot stand brengen. Zodra er een overeenkomst is bereikt, kunnen de data worden overgedragen. Het hele proces kan worden geautomatiseerd.

Het uitvoeren van contractonderhandelingen is veelal een (semi-)geautomatiseerd onderhandelingsproces, dat wordt uitgevoerd door de deelnemende data connectoren. De data connectoren beschikken daarvoor over een controlemechanisme voor het datagebruik. Daarbij wordt toegewerkt naar een contractovereenkomst over de dataset uitwisseling tussen de dataproducent en dataconsument. Figuur ? toont een eenvoudige versie van de procedure of processtappen, die ten minste nodig is om tot een contractovereenkomst te komen. Vooraf heeft de dataproducent een contractaanbod aan een dataset gekoppeld. Het contractaanbod wordt teruggestuurd naar de dataconsument als onderdeel van de metadata van de data connector. De dataconsument kan echter te allen tijde een contractaanvraag bij de dataprovider indienen, ook als nog geen contractaanbod bestaat.

<aside class='note' title="Implementatie-specifieke varianten op contractonderhandelingen">

Houd er rekening mee dat, aangezien dit een technologie-onafhankelijke berichtenstroom is, er geen rekening is gehouden met passende reacties. De geïllustreerde processen kunnen zowel synchroon als asynchroon worden uitgevoerd en kunnen op elk moment worden geannuleerd.
Contract onderhandelingen kunnen erg complex worden. Dit heeft mede te maken met het feit, dat het aantal policyvarianten met ODRL erg groot kan zijn. Bij de implementatie van een policy engine, die contractonderhandelingen mogelijk gemaakt worden hiervoor deterministische algoritmen gebruikt. Ook wordt gebruik gemaakt van een conceptueel kader van de OASIS XACML standaard [[XACML]] om contract onderhandelingen uit te voeren.  
</aside>

Indien de contractonderhandelingsprocedure wordt geïnitieerd door de dataconsument dan wordt door de connector van de dataconsument een contractaanvraag naar de dataproducent gestuurd. De inhoud van dit contractverzoek kan afwijken van het contractaanbod, of het kan het overnemen zoals het is. De informatie in het contract wordt dienovereenkomstig gewijzigd (bijv. de datum, de looptijd of de handtekening). Zodra de data connector van de dataproducent de contractaanvraag ontvangt, wordt de geldigheid ervan gecontroleerd door middel van syntaxis, inhoud en handtekening. Het contractverzoek wordt dus afgewezen of geaccepteerd. 
Indien het contractverzoek wordt geaccepteerd, dan wordt de contractovereenkomst ook ondertekend door de data connector van de dataproducent en wordt de dataconsument ter bevestiging geïnformeerd over de contractovereenkomst. 
Zodra er een contractovereenkomst is bereikt, wordt deze geïnstantieerd en geïmplementeerd binnen beide data connectoren, zowel die van de producent als van de dataconsument. Op deze manier beschikken beide connectoren over alle benodigde informatie voor latere beleidshandhaving (zie boven).
 
<figure id="Figuur_x">
<a href="media/IDS Vereenvoudigde weergave van de contractonderhandelingen.png" target="_blank"><img src="media/IDS Vereenvoudigde weergave van de contractonderhandelingen.png" alt=""></a>
<figcaption>Vereenvoudigde weergave van de contractonderhandelingen [[IDS-RAM4]]<figcaption>
</figure>

Als een deelnemer op enig moment tijdens de onderhandelingsprocedure niet akkoord gaat met de gedeelde inhoud, kan het contract worden afgewezen. In het geval van een afwijzing van een contract wordt de onderhandelingsprocedure afgebroken. De aangesloten systemen en gebruikers worden op de hoogte gebracht en eerder opgeslagen contractovereenkomsten worden ingetrokken. 
<br>

**Contractonderhandeling gestart door de producent**
<br>
De contractonderhandeling kan echter ook door de producent worden gestart. In figuur 10 start niet de consument, maar de producent de contractonderhandeling. Daarbij wordt opgemerkt dat, aangezien de producent degene is die het contract aanbiedt, de producent ook dan degene is die de contractovereenkomst als laatste ondertekent.  

<figure id="Figuur_x">
<a href="media/IDS Contractonderhandeling gestart door de producent.png" target="_blank"><img src="media/IDS Contractonderhandeling gestart door de producent.png" alt=""></a>
<figcaption>Contractonderhandeling gestart door de producent [[IDS-RAM4]]
  <figcaption>
</figure>

## Datatransfer

In de datatransferfase, als alle bovengenoemde processen met succes zijn afgerond, kunnen de producent en consument beginnen met het daadwerkelijk uitwisselen van data door een datatransfer methode aan te roepen, bijv. het uploaden of downloaden van een dataset, een datatransformatie of dataopvraging via hun data connectoren. 

Het uitvoeren van de data transfer begint met het aanroepen van een Data Operation verzoek in de control plane (zie figuur 11) en wordt geïnitieerd door een data connector die verwijst naar een contractovereenkomst. Aangezien de daaropvolgende sequentie niet gebonden mag zijn aan een communicatieprotocol of een communicatiepatroon, kan dit op verschillende manieren anders worden geïmplementeerd. Om dit te laten werken, heeft een Data Operation verzoek informatie nodig die technische automatisering mogelijk maakt (bijv. authenticatie-informatie of protocoldetails). 

 <figure id="Figuur_x">
<a href="media/IDS Globale procesbeschrijving data transfer.png" target="_blank"><img src="media/IDS Globale procesbeschrijving data transfer.png" alt=""></a>
<figcaption>Globale procesbeschrijving data transfer [[IDS-RAM4]]
  <figcaption>
</figure>
<br>

**Communicatiepatroon**
<br>
De communicatie tussen de data connectoren kan synchroon of asynchroon zijn. In het laatste geval hoeft de consument niet te wachten op het resultaat, maar wordt de consument door de provider op de hoogte wordt gebracht zodra het resultaat beschikbaar is. Bovendien kan er in plaats van een pull-request een push-request worden verstuurd. In het geval van een abonnement kan de consument vragen om updates met betrekking tot de gevraagde data. De bijgewerkte data kunnen worden verstrekt na bepaalde gebeurtenissen (bijv. nadat de data door de dataverstrekker zijn bijgewerkt) of binnen bepaalde tijdsintervallen (bijv. elke vijf minuten). Als er een dergelijk verzoek wordt gedaan, ontvangt de dataconsument herhaaldelijk bijgewerkte queryresultaten van de dataproducent. In het geval van een pull-request kan de dataconsument het laatste deel van het proces herhalen om data opnieuw op te vragen (met dezelfde of een andere query).
De beschrijving van het communicatiepatroon tijdens de data uitwisseling maakt geen deel uit van het Dataspace Protocol. Communicatie patronen, zoals het gebruik van downloadservices en API’s worden door vastgesteld door afspraken in de betreffende informatiedomeinen. De data-uitwisseling en het overdrachtsproces is dus niet beperkt tot een specifiek protocol. 

## Dataspace Protocol specificatie en data connector software

Het Dataspace Protocol is een technische specificatie, die de implementatie van het Dataspace Protocol in een data connector mogelijk maakt. Het Dataspace Protocol is een reeks van technische specificaties ontworpen om interoperabele data-uitwisseling mogelijk te maken gebaseerd op webtechnologieën. Deze specificaties definiëren de schema's (JSON) en het berichtenverkeer, die nodig zijn om de datasets te publiceren, overeenkomsten te onderhandelen en toegang te krijgen tot datasets binnen een dataspace. De huidige versie van de Dataspace Protocol specificatie wordt beschouwd als stabiel, en verdere wijzigingen zullen de conformiteit niet beïnvloeden ([[ECLPS-DSP]]). De specificaties zijn georganiseerd in verschillende onderdelen, waaronder:
1. Dataspace Model en Dataspace terminologie; 
2. Catalog protocol en catalog; 
3. Contractonderhandelingsprotocol en contractonderhandeling;
4. Data transfer protocol en data transfer proces.
We gaan hier niet verder in op de technische specificatie daarvoor verwijzen we naar ([[ECLPS-DSP]]).
<br>

**Data connector software**
<br>
Data connectors zijn softwaretools waarmee data(sets) vertrouwd kunnen worden gedeeld en geïntegreerd tussen verschillende systemen, applicaties en databronnen. In de context van data spaces spelen data connectoren een sleutelrol in de communicatie en gegevensuitwisseling tussen verschillende platforms, systemen en applicaties. Data connectoren zullen daarbij moeten voldoen aan de vooraf gedefinieerde normen en uitwisselingsbeleidslijnen van het Dataspace Protocol. In het data connectors overview report van IDSA [[IDS-DCR]] zijn inmiddels zo’n 40 verschillende implementaties van data connector software beschikbaar. implementaties van data connector software worden door IDSA gecertificeerd. Sinds 2022 hanteert IDSA het IDS-certificeringsschema dat gericht is op het certificeren van de interoperabiliteit, compatibiliteit en betrouwbaarheid van data connectoren. Met de voltooiing van de standaardisatie van het Dataspace Protocol zal het IDS-certificeringsschema evolueren om data connector software te beoordelen door  geautomatiseerde testen.

**TNO Security Gateway data connector software**
In dit experiment hebben we gekozen te werken met de data connector software van TNO, de TNO Security Gateway (TSG). De volgende overwegingen hebben daarbij een rol gespeeld:
1.	TSG is een IDSA-gecertificeerde implementatie (zie [[IDS-DCR]];
2.	TGS is open source software;
3.	Geonovum acteert binnen TNO’s Centre of Excellence for Data Sharing en Cloud (CoE-DSC)
Voor alle details over de implementatie van de TSG zie [[TNO-TSG]].


