# Experiment 2: DCAT metadata catalogi & data space connector 

## Inleiding 
In het data space protocol speelt de DCAT standaard een belangrijke rol om metadata van de aangeboden (geo)datasets te beschrijven. Het doel van experiment 2 is om DCAT metadata uitwisseling tussen de TSG data connector te testen met andere catalogus software, die DCAT ondersteunt: CKAN. 
Het idee daarbij is dat de catalogus, die gebruikt wordt voor de specifieke use case binnen de data space een subset van metadata uit een CKAN overneemt en in de catalogus van de data space publiceert. De catalogus, die daarvoor gebruikt wordt binnen deze use case is een CKAN catalogus. Daarnaast moet de metadata ook opgenomen worden in de TSG data space connector (als onderdeel van de data plane), zodat de relevante metadata gevonden kan worden als onderdeel van de data plane API interactie.

<aside class='note' title="Met dank aan het Kadaster">

Graag spreken de auteurs onze dank uit aan de Innovatieboard van het Kadaster voor het beschikbaar stellen van de financiële middelen, die de uitvoering van dit experiment mogelijk hebben gemaakt. Dankzij deze ondersteuning kon de DCAT metadata uitwisseling tussen metadata catalogi en de TSG data space connector in de praktijk beproeven. De bijdrage van het Innovatieboard heeft daarmee een belangrijke rol gespeeld in het verkennen van nieuwe mogelijkheden voor metadata-uitwisseling, interoperabiliteit en vindbaarheid binnen data spaces. De auteurs waarderen het vertrouwen en de ruimte die is geboden om te experimenteren en te leren.

</aside>

## Doel experiment
Doel van experiment 2 is te kijken in hoeverre DCAT metadata kan worden uitgewisseld vanuit enkele bestaande catalogi met de TSG data space connector. Om dit doel te bereiken onderzoeken en beschrijven we in dit experiment of DCAT metadata kan worden uitgewisseld tussen:
<ol>
  <li>CKAN met de catalogus van de TSG data space connector;</li>
  <li>CKAN met de federatieve catalogus van de SAGE Green Deal Data Space;</li>
  <li>CKAN met de federatieve catalogus van de SAGE Green Deal Data Space. </li>
</ol>

## Relevantie van het experiment
De relevantie van het experiment is meervoudig, omdat: 
<ol>
  <li>Het aantoont hoe DCAT effectief kan worden ingezet voor consistente metadata-uitwisseling binnen een data space;</li>
  <li>Het versterkt de interoperabiliteit tussen de TSG data space connector catalogus en bestaande broncatalogi, zoals CKAN, dat in veel publieke open data portals worden gebruikt;</li>
  <li>Het experiment laat zien hoe een data space een eigen catalogus kan opbouwen op basis van een gecontroleerde subset uit een broncatalogus;</li>
  <li>De integratie van metadata in de TSG data space connector toont hoe het control plane en data plane elkaar versterken binnen een data space architectuur;</li>
  <li>Organisaties krijgen inzicht in hoe zij bestaande DCAT metadata standaarden (profielen) optimaal kunnen benutten bij het vormgeven van data-uitwisselingsketens;</li>
  <li>Het experiment verkleint technische risico's rondom adoptie van DCAT en de Nederlandse [[DCAT-AP-NL]] en Europese profielen ([[DCAT-AP]] en [[geoDCAT-AP]]) in operationele data space implementaties.</li>
</ol>

## Opstelling experiment

De volgende vier use cases over het (her)gebruik en de uitwisseling van DCAT metadata zijn in deze paragraaf verder beschreven als use case beschrijving (precondities, actormodel, uit te voeren stappen en postcondities) en de technische implementatie en uitwerking:
<ol>
  <li>Use case 1 - DCAT metadata uitwisseling tussen CKAN en TSG data space connector;</li>
  <li>Use case 2 - Zoeken van de dataset in de TSG data space connector;</li>
  <li>Use case 3 - Harvesten van de CKAN vanuit de SAGE federated catalogus en publiceren van de metadata in de SAGE federated catalogus;</li>
  <li>Use case 4 - Het publiceren van de TSG data space connector in de SAGE participant Agent registry.</li>
</ol>

In onderstaande Figuur 18 is de opzet van het experiment weergegeven.

<figure id="Figuur_x">
<a href="media/Use case DCAT catalogs en TSG met pull-push v5.png" target="_blank"><img src="media/Use case DCAT catalogs en TSG met pull-push v5.png" alt=""></a>
<figcaption>Use cases DCAT catalogi en TSG data connector experiment<figcaption>
</figure>

Vanuit dit perspectief werken we aan we aan zes use cases (zie gebruiksfuncties in paragraaf 2.4.2) om te gaan met metadata in catalogi vooral vanuit het perspectief van de data provider, maar ook van de data consument:
<ol>
  <li>Het perspectief van de data provider, die metadata publiceert in de catalog service van de TSG data connector en gebruik maakt van een andere catalogus;</li>
  <li>Het perspectief van de consument, die een dataset zoekt, vindt en evalueert in de catalog service van de TSG data space connector.</li>
</ol>
<br/>
Het gaat daarbij specifiek om te beproeven hoe DCAT metadata van één of meerdere 'vertrouwde' datasets kan worden uitgewisseld tussen GeoNetwork en CKAN en tussen CKAN en de TNO Security Gateway, ook wel de data space connector. 
<br/>
Voor het uitvoeren van de zes use cases zijn bestaande metadata catalogi ingezet: 
<ol>
  <li>CKAN catalogus: <a href='https://sage.beta.geodan.nl/' target='_blank'>SAGE circulaire grondstromen</a></li>
  <li>Een lokale TSG data space connector setup specifiek voor dit experiment;</li>
  <li>De SAGE Federated Catalog. URL: pm;</li>
  <li>De SAGE Participant Agent registry. URL: pm.</li>
</ol>

Voor het uitvoeren van de use cases is gewerkt met de volgende software configuraties (zie onderstaande tabel).

<table>
  <colgroup>
    <col style="width: 20%;">
    <col style="width: 40%;">
    <col style="width: 40%;">
  </colgroup>
  <thead>
    <tr>
      <th><strong>Catalogi en data space connector</strong></th>
      <th><strong>Beschrijving</strong></th>
      <th><strong>GitHub URL</strong></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>CKAN</td>
      <td>Open data-catalogus met specifieke componenten voor geoDCAT metadata-uitwisseling</td>
      <td>
        https://github.com/NielsHoffmann/ckan-docker<br>
        of<br>
        https://github.com/sogelink-research/ckan-docker
      </td>
    </tr>
    <tr>
      <td>TSG data space connector</td>
      <td>TNO data space connector met DCAT-catalogus</td>
      <td>https://tsg.dataspac.es/</td>
    </tr>
    <tr>
      <td>Sogelink CKAN-TSG harvester</td>
      <td>CKAN-TSG harvesting- en search-engine-tool om metadata te raadplegen in de catalogus van de TSG data space connector</td>
      <td>https://github.com/sogelink-research/ckan-dataspace</td>
    </tr>
    <tr>
      <td>SAGE federated catalog</td>
      <td>pm</td>
      <td>pm</td>
    </tr>
    <tr>
      <td>SAGE Participant Agent registry</td>
      <td>pm</td>
      <td>pm</td>
    </tr>
  </tbody>
</table>


<aside class='note' title="Generieke stappen">

Voor het uitvoeren van de use cases worden minimaal de volgende stappen doorlopen: 
<ol>
  <li>Kiezen en zorgen voor relevante de endpoints voor het harvesten van metadata uit broncatalogi naar doelsysteem;</li>
  <li>Daarvoor configureren van het harvesting doelsysteem (andere catalogus of data space connector) met bron-URL (endpoint), filters (tags/thema's), interval of event-trigger en evt. beveiliging (authenticatie/authorisatie);</li>
</li>Voer mapping uit naar het doelsysteem; map DCAT-velden naar intern metadatamodel van bron- en doelsystemen (CKAN, TSG).
</li>
</ol>

</aside>

Binnen de experimenten met de DCAT catalogi en de data space connector is gebleken dat het op dit moment nog niet mogelijk was om met één uniform metadata-profiel te werken. Daarom is gekozen voor een pragmatische benadering, waarbij per situatie is beoordeeld welke vorm van metadata uitwisseling het meest passend en werkbaar was. Dit heeft ertoe geleid dat gebruik is gemaakt van meerdere DCAT-profielen, waaronder ISO19139, GeoDCAT en DCAT-AP-NL, in plaats van één enkel profiel. 

## Uitvoering

### Use case 1 - DCAT metadata uitwisseling tussen CKAN en TSG Data Connector ###

In use case 3 is beproefd hoe DCAT metadata uitwisseling kan plaatsvinden tussen CKAN (CKANNext-DCAT) en TSG data space connector. Daarvoor is de TSG data space connector aangepast om aanvullende metadata elementen uit [[DCAT-AP]], [[DCAT-AP-NL]] en [[geoDCAT-AP]] te ondersteunen. Aanleiding hiervoor was dat de TSG bij het publiceren van datasets oorspronkelijk alleen een beperkt aantal standaardattributen toestond, namelijk `@id`, `title`, `version` en `backendUrl` (zie onder). Daardoor was het niet mogelijk om rijkere beschrijvende metadata op te nemen, terwijl die juist nodig zijn om (geo)datasets goed vindbaar, interpreteerbaar en herbruikbaar te maken binnen een data space connector. 

Bij het publiceren van de metadata beschrijvingen van (geo)datasets in de TSG waren aanvankelijk alleen de volgende metadata attributen opvraagbaar:
<br/>

```json
{
  "@id": "123456",
  "title": "Test Dataset X",
  "version": "1.0.1",
  "backendUrl": "https://soilhub.beta.geodan.nl/gelderland/api/marketplace"
}
```

<br/>
De TSG data space connector hanteert een hiërarchische DCAT-structuur waarin een `Catalog` datasets en dataservices groepeert, en waarin onder een `Dataset` onder meer informatie over conformiteit, distributies en services kan worden vastgelegd (zie onder). In die opzet is ruimte voor verwijzingen naar standaarden, schema's, media types en endpoint beschrijvingen, maar in de oorspronkelijke implementatie konden deze aanvullende DCAT-elementen niet daadwerkelijk via de connector worden opgeslagen. Daarmee vormde de beperkte metadata-ondersteuning een belemmering voor toepassing van DCAT-profielen, zoals [[DCAT-AP-NL]] en [[geoDCAT-AP]].

<figure id="Figuur_x">
<a href="media/TSG Metadata (hierachie).png" target="_blank"><img src="media/TSG Metadata (hierachie).png" alt=""></a>
<figcaption>DCAT metadata elementen TSG dataspace connector<figcaption>
</figure>

Er was geen mogelijkheid om aanvullende metadata mee te geven, wat de toepassing van DCAT profielen binnen de TSG data space connector in de weg staat. Om dit op te lossen is vanaf versie 0.19.0 van de TSG software een nieuw veld toegevoegd: extraProps. Dit veld heeft het type object en maakt het mogelijk om bij het aanmaken of bijwerken van een dataset via de HTTP data plane aanvullende DCAT properties mee te geven. De uitbreiding maakt het mogelijk om naast de vaste basisattributen ook extra metadata op te slaan die relevant zijn voor nationale en domeinspecifieke DCAT profielen.

<br/>
Met deze aanpassing is de TSG data space connector beter bruikbaar geworden als catalogus component voor geodatasets binnen een DCAT-georiënteerde data space. De introductie van extraProps biedt een generiek uitbreidingsmechanisme waarmee aanvullende elementen uit DCAT AP-NL en geoDCAT kunnen worden opgenomen zonder dat voor ieder nieuw attribuut afzonderlijk aanpassingen in het datamodel nodig zijn. Daarmee is een belangrijke stap gezet richting rijkere metadata registratie en een betere aansluiting op gangbare interoperabiliteitsprofielen voor metadata afgestemd op de Nederlandse ([[DCAT-AP-NL]]) en Europese ([[geoDCAT-AP]]) situatie.

<br/>
Voor documentatie over de DCAT 'custom properties' en `extraProps` en de toegepaste API informatie van de TSG data space connector zie de onderstaande tabel. 

<table>
  <colgroup>
    <col style="width: 40%;">
    <col style="width: 60%;">
  </colgroup>
  <thead>
    <tr>
      <th><strong>TSG data space connector</strong></th>
      <th><strong>Informatie via URL</strong></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Custom DCAT Properties / Application Profiles</td>
      <td>https://tsg.dataspac.es/docs/next/architecture/dcat-structure#custom-dcat-properties-application-profiles</td>
    </tr>
    <tr>
      <td>Dataset configuratie: <code>extraProps</code></td>
      <td>https://tsg.dataspac.es/docs/next/deployment/dataset#custom-dcat-properties-extraprops</td>
    </tr>
    <tr>
      <td>Dataset aanmaken: <code>data-plane-management-controller-create-dataset</code></td>
      <td>https://tsg.dataspac.es/docs/next/apis/http-data-plane/data-plane-management-controller-create-dataset</td>
    </tr>
    <tr>
      <td>Dataset bijwerken: <code>data-plane-management-controller-update-dataset</code></td>
      <td>https://tsg.dataspac.es/docs/next/apis/http-data-plane/data-plane-management-controller-update-dataset/</td>
    </tr>
  </tbody>
</table>

**JSON voorbeeld: metadata aanmaken met `extraProps` (conform [[DCAT-AP-NL]])**

Onderstaand JSON-voorbeeld laat zien hoe metadata bij het aanmaken van een dataset kan worden uitgebreid met het veld `extraProps`. Hiermee kunnen aanvullende eigenschappen worden meegegeven die aansluiten op [[DCAT-AP-NL]] v3.0, zodat naast de standaard datasetvelden ook rijkere en profielspecifieke metadata in de TSG data space connector kunnen worden opgeslagen.
<br/>
```json
{
  "@id": "dataset-bodemkaart-gelderland",
  "title": "Bodemkaart Gelderland",
  "version": "1.0.0",
  "backendUrl": "https://soilhub.beta.geodan.nl/gelderland/api/marketplace",
  "extraProps": {
    "dct:description": "Bodemkaart van de provincie Gelderland met bodemtype-informatie per perceel.",
    "dct:identifier": "https://data.geodan.nl/datasets/bodemkaart-gelderland",
    "dct:issued": "2024-01-15",
    "dct:modified": "2024-06-01",
    "dct:language": "http://publications.europa.eu/resource/authority/language/NLD",
    "dct:license": "http://creativecommons.org/licenses/by/4.0/",
    "dct:publisher": {
      "@id": "https://www.geodan.nl",
      "foaf:name": "Geodan"
    },
    "dct:spatial": {
      "@type": "dct:Location",
      "locn:geometry": {
        "@type": "gsp:wktLiteral",
        "@value": "POLYGON((5.5 51.6, 7.1 51.6, 7.1 52.5, 5.5 52.5, 5.5 51.6))"
      }
    },
    "dct:temporal": {
      "@type": "dct:PeriodOfTime",
      "dcat:startDate": "2020-01-01",
      "dcat:endDate": "2023-12-31"
    },
    "dcat:keyword": ["bodem", "bodemkaart", "Gelderland", "percelen"],
    "dcat:theme": "http://publications.europa.eu/resource/authority/data-theme/ENVI",
    "dcat:contactPoint": {
      "@type": "vcard:Organization",
      "vcard:fn": "Geodan Datateam",
      "vcard:hasEmail": "mailto:data@geodan.nl"
    },
    "dqv:hasQualityMeasurement": {
      "@type": "dqv:QualityMeasurement",
      "dqv:isMeasurementOf": "https://www.w3.org/TR/vocab-dqv/#completeness",
      "dqv:value": 0.95
    }
  }
}
```
<br/>
Het experiment demonstreert hoe metadata records uit een CKAN catalogus geoogst kunnen worden voor opname en ontsluiting in de catalogus van de TSG data space connector. Hiervoor zijn metadata beschrijvingen van datasets uit de <a href='(https://dataportals.org/portal/amsterdam_open_data/) 'target='_blank'>CKAN catalogus van de Gemeente Amsterdam</a> als uitgangspunt gebruikt. Daarvoor zijn metadata records van een set (geo)datasets van een CKAN catalogus van de Gemeente Amsterdam eerst is geïmporteerd in een voor dit experiment ingerichte CKAN instantie voor <a href='https://sage.beta.geodan.nl/' target='_blank'>SAGE circulaire grondstromen</a>. 
<br/>

Met het onderstaande commando wordt vanuit CKAN  metadata records naar de catalogus van de  TSG overgestuurd. 
<br/>

`npm run add:ckan`

<br/>

Na het uitvoeren van de CKAN-TSG harvester zijn de metadata records van de CKAN instantie via een pull- en push-mechanisme overgehaald. De volgende stappen zijn daarbij doorlopen voor de export naar metadata records van CKAN naar de TSG data space connector: 
<ol>
  <li>Via een pull-mechanisme is de `.jsonld`-extensie (de standaard CKAN-exportfunctie voor linked data) is de metadata geëxporteerd uit CKAN in [[DCAT-AP-NL]] 3.0 formaat</li>
  <li>Het JSON-LD-bestand is vervolgens gebruikt om de metadata van datasets aan te maken in de data space connector via het `extraProps` veld van de TSG HTTP data plane API;</li>
</li>Via het data plane management van de TSG data space connector zijn de JSON-LD-bestanden vervolgens bijgewerkt via de beschikbare TSG API’s voor data plane management (controller-create-dataset of controller controller-update-dataset).
</li>
</ol>
<br/>
Tijdens het uitvoeren van de CKAN-TSG harvester laat de command line interface (CLI) zien, dat de metadata records (in totaal 347 records) van uiteenlopende (geo)datasets daadwerkelijk uit de CKAN broncatalogus van de gemeente Amsterdam worden opgehaald en verwerkt (zie figuren onder). In de uitvoer is per dataset zichtbaar dat de metadata wordt ingelezen en doorgezet naar de TSG-omgeving. Deze CLI-meldingen bevestigen daarmee dat het harvestproces actief is en dat de overdracht van datasets tussen CKAN en TSG technisch functioneert zoals bedoeld.

<figure id="Figuur_x">
<a href="media/Harvesting CKAN-TSG-CLI_1.png" target="_blank"><img src="media/Harvesting CKAN-TSG-CLI_1.png" alt=""></a>
<figcaption>Start run CKAN-TSG harvester<figcaption>
</figure>

<figure id="Figuur_x">
<a href="media/Harvesting CKAN-TSG-CLI_2.png" target="_blank"><img src="media/Harvesting CKAN-TSG-CLI_2.png" alt=""></a>
<figcaption>Einde run van de CKAN-TSG harvester<figcaption>
</figure>

<aside class='note' title="Andere Ckan instantie gebruiken?">

In de programmatuur is nu een Ckan instantie van de gemeente Amsterdam opgenomen. Met deze programmatuur kunnen ook andere Ckan instanties worden bevraagd en metadata uitwisselen met de TSG data space connector. Maar daarvoor dient een URL aanpassing plaats te vinden. Als de URL wordt aangepast, dan wordt een andere CKAN-instantie bevraagd. Maar om goed te werken, moet de CKAN-instantie wel zijn geconfigureerd om JSON-LD te leveren. Voor de remote CKAN instantie is minimaal nodig:
<ol>
  <li>ckanext-dcat inschakelen</li>
  <li>
    Een DCAT/GeoDCAT-endpoint publiceren dat JSON-LD retourneert. Dit is de URL die in de CKAN-TSG connector moet worden ingesteld.
  </li>
  <li>
    Sterk aanbevolen voor metadata met geografische kenmerken en bevragingen:
    <ul>
      <li><code>ckanext-spatial.</code>Voor ruimtelijke velden zoals <code>bbox</code> en <code>centroid</code></li>
      <li><code>ckanext-scheming.</code>Voor extra geo-metadata via een custom schema</li>
    </ul>
  </li>
</ol>
Een voorbeeld van zo'n CKAN configuratie voor docker staat op https://github.com/sogelink-research/ckan-docker.
</aside>

### Use case 2 - Zoeken in de TSG data space connector catalogus ###

We hebben in de vorige twee use cases metadata toegevoegd vanuit de metdata catalogus CKAN aan de catalogus van de TSG data space connector. Hoe kunnen we nu de metadata doorzoeken in de TSG data space connector? De TSG data space connector heeft een mogelijkheid om de metadata records te bekijken via de TSG GUI (zie onderstaande figuren). 

De TSG user interface (UI) voor het zoeken raadplegen van de aanwezige metadata records in vrij beperkt (daar is de TSG ook niet voor ontwikkeld).  Hieronder het scherm om de metadata in te zien; de Versions (metadata elementen `Indentifier`, `Version`, `Message model URL` en `Authorisation`). En daaronder de Policy uitgedrukt in ODRL JSON-LD. 

<figure id="Figuur_x">
<a href="media/TSG HTTP Data Plane.png" target="_blank"><img src="media/TSG HTTP Data Plane.png" alt=""></a>
<figcaption>DCAT metadata elementen in TSG data space connector<figcaption>
</figure>

Het doorzoeken van de metadata is in de TSG UI gaat via de Tester en het laden van de reload catalog. Deze geeft een overzicht van de Participants Agents (beschikbare data space connectors) en vervolgens wordt een overzicht gegeven van de datasets (‘http datasets’). Dat levert een lijst op van de (geo)datasets.

<br/>
<figure id="Figuur_x">
<a href="media/TSG HTTP Data Plane DCAT Metadata records.png" target="_blank"><img src="media/TSG HTTP Data Plane DCAT Metadata records.png" alt=""></a>
<figcaption>Zoeken van metadata records met de TSG data space connector<figcaption>
</figure>
<br/>

Binnen het experiment met de DCAT data space connector is naast het opslaan van aanvullende metadata ook gekeken naar het doorzoekbaar maken van de beschikbare metadata in de TSG data space connector. Het doel hiervan was om niet alleen datasets en bijbehorende metadata in de TSG catalogus op te nemen, maar deze ook op een toegankelijke manier te kunnen zoeken, vinden en bekijken. Hiervoor is een zoekinterface gemaakt, die de TSG data space connector bevraagd. Met deze zoekinterface kunnen metadata van (geo)datasets, die eerder via harvesting of publicatie in de TSG data space connector catalogus zijn opgenomen, worden geraadpleegd. Daarmee is een praktische voorziening gerealiseerd om de inhoud van de catalogus beter te ontsluiten en de bruikbaarheid van de opgeslagen DCAT-metadata te vergroten. 
<br/>

Na het harvesten van de metadata kan vervolgens de search engine portal worden gestart: 
<br/>

`npm run portal`

<br/>
De TSG data space 'portal' geeft inzicht in de metadata van alle datasets, zoals ze opgenomen in de lokale instantie van de TSG. In onderstaande figuur gaat het om 374 metadata records die zijn opgehaald. Met de portal kan via de zoekinterface gerichter gezocht worden naar datasets en de meegekomen metadata kan daarbij worden opgevraagd.  
Daarmee ontstaat een eenvoudige gebruikersinterface waarmee de in de TSG-catalogus beschikbare datasets en hun metadata kunnen worden doorzocht en ingezien. Deze laat zien dat de TSG data space connector niet alleen kan functioneren als opslag- en uitwisselcomponent voor DCAT-metadata, maar ook als basis voor een doorzoekbare catalogusvoorziening. Dat is relevant voor dataspaces waarin het niet voldoende is om metadata alleen te registreren, maar waarin deze ook snel vindbaar en inspecteerbaar moeten zijn voor gebruikers en applicaties.

<figure id="Figuur_x">
<a href="media/TSG dataspace Portal.png" target="_blank"><img src="media/TSG dataspace Portal.png" alt=""></a>
<figcaption>User interface van de zoekclient TSG data space 'Portal'<figcaption>
</figure>

<figure id="Figuur_x">
<a href="media/TSG dataspace Portal Zoeken UI.png" target="_blank"><img src="media/TSG dataspace Portal Zoeken UI.png" alt=""></a>
<figcaption>Zoeken en opvragen van DCAT metadata met de zoekclient 'TSG dataspace Portal'<figcaption>
</figure>

In deze use case is onderzocht hoe DCAT metadata van datasets kan worden gebruikt binnen de TSG data space connector. De centrale vraag was: in hoeverre is het mogelijk om rijke DCAT-metadata te koppelen aan datasets, die worden gepubliceerd in de catalogus van een TSG data space connector. En vervolgens ook deze metadata te kunnen bekijken. Het zoeken in de catalogus van de data space connector is geïmplementeerd via een specifieke zoekclient, die op basis van de DCAT metadata die is opgeslagen in het `extraProps` veld, de datasets in catalogus van de data space connector kan vinden en tonen. 
<br/>
Er zijn twee beperkingen aan het zoeken met deze zoekclient: 
<ol>
  <li>Beperkt zoekbereik. bij het zoeken wordt geen zoekactie gestart bij alle participanten in de data space; het zoeken is beperkt tot één participant tegelijk;</li>
  <li>Alleen tekstueel zoeken. Er is geen ondersteuning voor ruimtelijke zoekopdrachten, zoals het filteren van datasets op basis van een geografisch gebied (bounding box).
  </li>
</ol>
<br/>
Deze <a href='https://github.com/sogelink-research/ckan-dataspace/' target='_blank'>TSG catalogus zoekclient</a> is ontwikkeld door Sogelink Research en is gedocumenteerd op github.

### Use case 3 - Harvesten van de CKAN vanuit de SAGE federated catalogus en publiceren van de metadata in de SAGE federated catalogus ###

In deze use case wordt beschreven hoe metadata uit de CKAN instantie, beschikbaar wordt gesteld via DCAT, en kan worden gepubliceerd naar de federated catalogus van <a href='https://www.greendealdata.eu/' target='_blank'>SAGE - The Data Space for a Sustainable Green Europe</a>. Het publiceren van deze metadata is een belangrijke stap om datasets niet alleen lokaal beschikbaar te maken, maar ook federatief vindbaar te laten zijn binnen een grotere data space. Daarmee wordt het mogelijk om datasets uit verschillende bronnen op een uniforme manier te ontsluiten en te hergebruiken.

Binnen deze use case speelt de CKAN catalogus van circulaire grondstromen een centrale rol als schakel tussen de bronmetadata en de federatieve catalogus. 
<br/>

pm

### Use case 4 - Het publiceren van de TSG data space connector in de Participant Agent Register ###

Ook de TSG data space connector maakt het mogelijk om DCAT metadata uit CKAN op te nemen, te verrijken en vervolgens beschikbaar te stellen binnen de data space context. Om deze rol goed te kunnen vervullen, is het niet alleen van belang dat de metadata correct wordt gepubliceerd naar de federated catalogus, maar ook dat de connector zelf als deelnemende component herkenbaar is binnen de data space. Daarom wordt de TSG data space connector ook worden geregistreerd in het Participant Agent Register van <a href='https://www.greendealdata.eu/' target='_blank'>SAGE - The Data Space for a Sustainable Green Europe</a>. Deze registratie is nodig om de connector als deelnemer binnen de SAGE Green Deal Data Space te identificeren en vindbaar te maken. Pas wanneer zowel de metadata in de federated catalogus is gepubliceerd als de data space connector in het Participant Agent Register is opgenomen, is sprake zijn van een goed aangesloten en vindbare (geo)datasets in de data space. 
<br/>

pm

## Opgedane bevindingen

In dit experiment is onderzocht in hoeverre DCAT metadata uit bestaande catalogi uitgewisseld kunnen worden met de DCAT catalogus  van de TNO Security Gateway data space connector  . Aanvankelijk bleek dat bij het publiceren van (geo)datasets alleen een beperkt aantal DCAT metadata velden beschikbaar was, zoals `identificatie`, `titel`, `versie` en `backend-URL`. Daardoor was het niet mogelijk om uitgebreidere metadata volgens DCAT profielen, zoals GeoDCAT-AP  mee te geven.
Met de introductie van het veld `extraProps` in versie 0.19.0 van de TSG data space connector software is daarin verandering gekomen. Dit nieuwe veld maakt het mogelijk om aanvullende DCAT eigenschappen vanuit bijvoorbeeld GeoDCAT-AP op te nemen bij het aanmaken of bijwerken van metadatata van geodatasets. Eerst is de metadata geïmporteerd in een CKAN-omgeving. Daarna is deze metadata in DCAT-AP-NL 3.0-formaat geëxporteerd als JSON-LD en via het veld `extraProps` opgenomen in de catalogus van de TSG data space connector. Vervolgens is aangetoond dat deze metadata binnen de data space beschikbaar is en gebruikt kan worden om datasets te doorzoeken.

Kortom, via de `extraProps`-optie in TNO TSG is het mogelijk om extra DCAT-metadata mee te sturen bij het aanmaken van een dataset in de HTTP data plane. Deze metadata kan vervolgens binnen de data space worden opgehaald en doorzocht. De werking van deze functionaliteit is gedemonstreerd, waarbij metadata van datasets zijn gepubliceerd vanuit een CKAN catalogus in de catalogus van de TSG data space connector en vervolgens doorzocht via specifieke TSG zoekclient. De implementatie toont aan dat het gebruik van rijkere DCAT metadata binnen een data space connector technisch haalbaar is, met als kanttekening dat de huidige zoekfunctionaliteit beperkte zoekmogelijkheden biedt; zoeken gebeurt niet tegelijk over meerdere data space connectoren, de 'participants' agents in een data space, en ruimtelijke zoekmogelijkheden ontbreken bijvoorbeeld.


