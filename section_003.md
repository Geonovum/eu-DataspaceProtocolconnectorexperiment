# Opzet experiment {#01340370}

## Systeemopzet van de minimum viable dataspace {#001BD7C0}
Ons experiment is bedoeld om te verifiëren of we een gegevensoverdracht kunnen realiseren tussen twee connectors binnen een dataspace-ecosysteem. Binnen dit ecosysteem kan elke dataspace-connector fungeren als gegevensaanbieder, consument of beiden. Bovendien zijn connectors gekoppeld aan dataspace-deelnemers (participants), die mensen, instellingen, bedrijven of mogelijk overheden kunnen zijn. In onze specifieke opzet implementeren we één gegevensaanbieder, genaamd `Alfa`, en één consument, genaamd `Bravo`, onder dezelfde deelnemer voor simulatie-doeleinden. We voeren een HTTP-verzoek uit met behulp van de OGC API.

## TNO Security Gateway (TSG) {#6193360E}
De TNO Security Gateway is een kant-en-klare implementatie van dataspace-componenten die door TNO worden aangeboden. De documentatie die bij het project wordt geleverd, legt uit hoe een volledig werkend dataspace-ecosysteem op een eigen cloudomgeving kan worden geïmplementeerd. Heronder richten we ons op de modulaire indeling van de dataspace-connector zoals beschreven door TNO:

- **Control Plane**
- **HTTP Data Plane**
- **Wallet**

Elke module heeft fundamentele functies en kan niet worden weggelaten in de context van een minimale en functionele dataspace-connector. Bovendien heeft elke module na een basisimplementatie van TNO zijn eigen dashboard-service. We zullen deze dashboards gebruiken om de basisworkflow en het experiment binnen een dataspace te demonstreren.

### TSG Control Plane {#4125B625}
De control plane fungeert als het "brein" van een dataspace-connector en stelt ons in staat het grootste deel van de functionaliteiten van het dataspace-protocol uit te voeren. Het biedt onder andere authenticatie door een token te genereren dat een vastgestelde tijd geldig is en dat kan worden gebruikt voor verdere acties. Na authenticatie kunnen we catalogi bekijken, een onderhandeling starten met een andere connector (bijvoorbeeld als gegevensaanbieder) en eventueel overgaan tot een gegevensoverdracht.

### TSG HTTP Data Plane {#5EC97A70}
De data plane fungeert als tegenhanger van de control plane voor een specifieke connector. Simpel gezegd volgt het de instructies van de control plane met betrekking tot gegevensoverdracht. Als het wordt gebruikt als consument, stelt het ons in staat directe gegevensdownloads uit te voeren of gegevens op te halen via API-requests van de data plane van een aanbieder.

### TSG Wallet {#726B0216}
De wallet bevat de verifieerbare referenties voor elke deelnemer binnen de dataspace. Een deelnemer kan aan meerdere connectors worden gekoppeld, maar andersom is dit niet het geval. Een centrale wallet (of meerdere wallets) geeft referenties uit aan deelnemers binnen het dataspace-ecosysteem.

## Functies en processen van de minimum viable dataspace {#01C8311E}
In deze sectie beschrijven we de kernstappen die nodig zijn voor een gegevensoverdracht tussen twee connectors die afzonderlijk optreden als consument en aanbieder.

### Onboarding door producent en consument {#4D30B938}

### Dataproducten aanbieden {#32BDC7C7}

### Bekijken en wijzigen van condities (‘policies’) {#143AA289}
We laten zien hoe regels kunnen worden gewijzigd voor de dataset `BravoHTTPBin` van `Bravo`. Je kunt vrijelijk toestemmingen en verboden toevoegen.

<img src='media/section_003/change-rules-dataset.png' alt='Verander regels voor dataset' style='width: 100%;'></img>

### Zoeken van catalogi van andere aanbieders (participanten) {#59F4CA7D}

### Zoek dataproducten in de catalogus {#79E15E32}
In de `Registry` binnen de control plane van een connector kunnen we de lijst vinden van gegevensbronnen die worden aangeboden door de huidige connector en de externe connectors waarvan onze connector op de hoogte is.

<img src='media/section_003/browsing-catalog.png' alt='Catalogus doorzoeken vanaf consument' style='width: 100%;'></img>

In het voorbeeld zien we de dataset `Bravo HTTPBin` dat toebehoort aan de consument `Bravo` evenals `Kadaster Percelen` en `Alfa HTTPBin` die toebehoren aan `Alfa`.

### Contractonderhandeling producent en consument {#288808F5}
De onderhandeling over een contract met betrekking tot een specifiek dataproduct omvat meerdere stappen tussen de consument en aanbieder. Eerst stuurt de consument `Bravo` een onderhandelingsverzoek naar de aanbieder `Alfa` zoals hieronder weergegeven.

<img src='media/section_003/contract-negotiation.png' alt='Contractonderhandeling versturen' style='width: 100%;'></img>

Nu beslist de aanbieder `Alfa` of hij de ontvangen onderhandeling van `Bravo` wil accepteren.

<img src='media/section_003/accept-negotiation.png' alt='Onderhandeling accepteren' style='width: 100%;'></img>

Bij acceptatie, en na ondertekening en tegenondertekening op beide control planes, mag `Bravo` uiteindelijk de gegevensoverdracht aanvragen zoals in de volgende afbeelding wordt getoond.

<img src='media/section_003/request-transfer.png' alt='Overdracht aanvragen' style='width: 100%;'></img>

### Gegevensoverdracht tussen producent en consument {#7BC4931F}
Zodra de consument de overdracht aanvraagt bij de aanbieder, wordt de overdracht als gestart beschouwd en blijft "open" totdat deze door een van de betrokken partijen als `Beëindigd` of `Voltooid` wordt gemarkeerd.

<img src='media/section_003/initiated-transfer.png' alt='Gestarte gegevensoverdracht' style='width: 100%;'></img>

Wat betekent "open"? Het betekent dat daadwerkelijke gegevensoverdrachten kunnen worden uitgevoerd tussen de data planes van de consument en aanbieder. Om echt gegevens van aanbieder `Alfa` naar consument `Bravo` te verplaatsen, moeten we authenticeren op de interface van de data plane van de consument en een specifiek HTTP-verzoek doorsturen naar de API van de aanbieder. In dit geval gebruiken we de OGC API-endpoint die beschikbaar is via de Kadaster data plane van `Alfa` om een verzameling Nederlandse gebouwen op te vragen.

<img src='media/section_003/http-request-params.png' alt='Verzoek sturen naar aanbieder' style='width: 100%;'></img>

De response van het verzoek ziet er dan als volgt uit:

<img src='media/section_003/http-request-response.png' alt='Respons ontvangen van aanbieder' style='width: 100%;'></img>
