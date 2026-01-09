# Experiment 2: Data connector catalogus & DCAT AP NL metadata

## Inleiding 
In de IDS data connector speelt de DCAT standaard een belangrijke rol om metadata van de aangeboden datasets te beschrijven. Het doel van het experiment is om DCAT metadata uitwisseling tussen de IDS data connector (TSG) te testen met andere catalogi die DCAT ondersteunen: het Nationaal georegister (NGR) en de catalogus circulaire grondstromen. We werken daarbij verder aan de bestaande praktijk casus uitgaande van een minimal viable data space met een ‘vertrouwde’ dataset van het Kadaster (‘eigendomskaart’).  
Het idee daarbij is dat de catalog, die gebruikt wordt voor de specifieke use case binnen de dataspace een subset van metadata uit het NGR overneemt en in de ‘eigen’ catalogus van de dataspace publiceert. De catalogus die daarvoor gebruikt wordt binnen deze use case is een CKAN catalogus. Daarnaast moet de metadata ook opgenomen worden in de TSG Connector (als onderdeel van het ‘control plane’), zodat de relevante metadata gevonden kan worden als onderdeel van de ‘data plane’ API interactie.

## Doel experiment
Doel van experiment 2 is te kijken in hoeverre DCAT3 metadata volgens DCAT AP NL van een ‘vertrouwde’ dataset kan worden uitgewisseld vanuit enkele bestaande catalogi volgens het DCAT AP NL profiel met de TSG data connector.  Om dit doel te bereiken onderzoeken we in dit experiment of DCAT3 metadata van één ‘vertrouwde’ dataset kan worden uitgewisseld tussen:
<ol>
  <li>Het nationaal georegister (Geonetwork met DCAT formatter) en de IDS data connector (TNO TSG);</li>
  <li>Het nationaal georegister (Geonetwork met DCAT formatter) en Catalog van Circulaire grondstromen (CKAN met CKANext-DCAT);</li>
  <li>Catalog van Circulaire grondstromen (CKAN met CKANext-DCAT); met CKAN en de IDS data connector (TNO TSG).</li>
</ol>
<br/>
In onderstaande Figuur ? is een eerste opzet van het experiment weergegeven.

<figure id="Figuur_x">
<a href="media/Use case DCAT catalogs en TSG met pull-push.jpg" target="_blank"><img src="media/Use case DCAT catalogs en TSG met pull-push.jpg" alt=""></a>
<figcaption>Opzet Data catalogs en IDS data connector experiment<figcaption>
</figure>

Vanuit dit perspectief werken we aan we aan twee use cases (zie gebruiksfuncties in paragraaf 2.4.2) om te gaan met metadata in catalogi:
<ol>
  <li>Het perspectief van de data provider, die metadata publiceert in de catalog service van de IDS data connector en gebruik maakt van een andere catalogus;</li>
  <li>HHet perspectief van de consument, die een dataset zoekt, vindt en evalueert in de catalog service van de IDS data connector.</li>
</ol>

## Relevantie van het experiment
De relevantie van het experiment is meervoudig, omdat: 
<ol>
  <li>Het aantoont hoe DCAT-AP-NL 3 effectief kan worden ingezet voor consistente metadata-uitwisseling binnen een data space;</li>
  <li>Het versterkt de interoperabiliteit tussen de IDS data connector catalogus en bestaande broncatalogi, zoals NGR (Geonetwork) en CKAN, die in veel overheidsdomeinen worden gebruikt;</li>
  <li>Het experiment laat zien hoe een data space een eigen catalogus kan opbouwen op basis van een gecontroleerde subset uit een broncatalogus;</li>
  <li>De integratie van metadata in de TSG Connector toont hoe het control-plane en data-plane elkaar versterken binnen een IDS-gebaseerde architectuur;</li>
  <li>Organisaties krijgen inzicht in hoe zij bestaande DCAT metadata standaarden (profielen) optimaal kunnen benutten bij het vormgeven van data-uitwisselingsketens;</li>
  <li>Het experiment verkleint technische risico’s rondom adoptie van DCAT en DCAT-AP-NL in operationele data space implementaties.</li>
</ol>

## Opstelling experiment
pm

## Uitvoering
Het gaat daarbij specifiek om te kijken of DCAT3 metadata conform DCAT AP NL van één of meerdere ‘vertrouwde’ datasets kan worden uitgewisseld tussen: 1. Geonetwork met DCAT Transformer (toegepast in het nationaal georegister), de TNO Security Gateway of TSG (data space protocol compliant connector) en CKAN met CKANNext-DCAT (de catalogus van circulaire grondstromen). 

**Use cases**
De volgende vijf use cases over het (her)gebruik en de uitwisseling van DCAT metadata zijn in deze paragraaf verder beschreven als use case beschrijving (precondities, actormodel, uit te voeren stappen en postcondities) en de technische implementatie en uitwerking:
<ol>
  <li>Use case 1 – Publiceren van een ’vertrouwde’ dataset in het Nationaal Georegister  (GeoNetwork) en via DCAT3-endpoint beschikbaar stellen (M2M) en via file download (H2M);</li>
  <li>Use case 2 – Metadata-uitwisseling (via DCAT3) tussen Nationaal Georegister (GeoNetwork) en Catalogus Circulaire Grondstromen (CKAN + CKANNext-DCAT) met variant 2.1 via file upload (human-to-machine) en variant 2.2 via harvesting DCAT3-endpoint (machine-to-machine);</li>
  <li>Use case 3 – Metadata-uitwisseling tussen Catalogus Circulaire Grondstromen (CKAN + CKANNext-DCAT) en IDS Data Connector (TSG) met variant 3.1 via file upload (human-to-machine) en variant 3.2 via harvesting DCAT3-endpoint (machine-to-machine);</li>
  <li>Use case 4 - Metadata-uitwisseling tussen het Nationaal Georegister  (GeoNetwork) en IDS Data Connector (TSG) met variant 4.1 via file upload (human-to-machine) en variant 4.2 via harvesting DCAT3-endpoint (machine-to-machine);</li>
  <li>Use case 5 – Zoeken van de dataset in de IDS Data Connector (TSG) door de consumer via de consumer IDS data connector (ook TSG).</li>
</ol>
<br/>

<aside class='note' title="Generieke stappen in alle use cases">
Onderstaande generieke stappen gelden feitelijk voor alle vijf use cases:
<li>Publiceer dataset in broncatalogus:
•	Vul DCAT3-compatibele metadata volledig in volgens één standaard profiel nl. DCAT AP NL;
•	Markeer dataset als “vertrouwd” en/of “in scope” voor uitwisseling.<li>
<li>Zorg voor DCAT3-/DCAT-AP-endpoint:
•	Broncatalogus biedt een stabiele DCAT3-feed (catalogusniveau of per dataset).<li>
<li>Configureer harvesting of push-mechanisme:
•	Doelsysteem (andere catalogus of IDS Connector) wordt geconfigureerd met:
•	bron-URL (DCAT endpoint),
•	filters (tags/thema’s),
•	interval of event-trigger,
•	beveiliging (authn/authz).<li>
<li>Voer mapping uit naar doelsysteem:
•	Map DCAT3-velden naar intern metadatamodel van bron- en doelsystemen (GeoNetwork, CKAN, TSG). <li>
<li>Maak of update resource in doelsysteem:
•	Maak nieuwe record of werk bestaande bij.
•	Bewaar verwijzing naar bron (URI).
<li>Beheer lifecycle en updates:
•	Wijzigingen in de broncatalogus worden periodiek gesynchroniseerd via dezelfde DCAT3-mechanismen.
</aside>
<br/>

### Use case 1 – Publiceren van een ‘vertrouwde’ dataset in NGR en beschikbaar stellen via DCAT3-endpoint (M2M) en file download (H2M) ###

Een provider publiceert een vertrouwde dataset in het Nationaal Georegister (NGR, GeoNetwork). De metadata voldoet aan het Nederlandse profiel voor en wordt DCAT AP NL. De metadata van de dataset is op twee wijzen beschikbaar:
•	via een DCAT3-endpoint (voor M2M interactie); en
•	als DCAT3-bestand (voor download door de mens).
<br/>
*Actormodel*
•	Datapublisher (mens);
•	Nationaal Georegister (NGR) – GeoNetwork + DCAT Transformer;
•	Externe systemen (CKAN, IDS Data Connector) – consumer van de DCAT3-metadata.
•	Eindgebruiker (mens) downloadt DCAT3-file.
<br/>
*Precondities*
•	Datapublisher heeft rechten in NGR;
•	DCAT Transformer is geconfigureerd voor DCAT AP NL / DCAT3;
•	Mechanisme om datasets als ‘vertrouwd’ te markeren is ingericht (bijv. tag, extra veld, policy URI);
•	Dataset zelf (dataresource) is technisch ergens hostbaar (bijv. WMS/WFS/REST/API of file).
<br/>
*Uit te voeren stappen*

1. Aanmaken en invullen metadata in NGR 
  1.1 Datapublisher logt in op NGR.
  1.2 Maakt een nieuw metadatasjabloon aan (gebaseerd op DCAT AP NL-profiel of NGR-profiel dat daarop mapt).
  1.3 Vult minimaal de verplichte velden:
  •	dct:title, dct:description, dct:identifier, dct:publisher
  •	dct:creator, dct:issued, dct:modified
  •	dct:license, dct:accessRights, evt. odrl:hasPolicy
  •	dcat:theme, dcat:keyword
  •	dct:spatial, dct:temporal
  •	dcat:distribution (met toegangspunten: download-URL, service-URL, API endpoint, formaat).
2.	Markeren als ‘vertrouwde’ dataset 
2.1 Datapublisher zet een veld/tag, bijv.:
•	Tag: trusted=true of ids-trusted.
•	Extra veld: vertrouwensniveau=vertrouwd.
•	Verwijzing naar een vertrouwens- of security policy in een URI veld.
2.2 Dit veld/tag wordt later gebruikt als filter door harvesters of import-scripts.
3.	Publiceren in NGR
3.1 Datapublisher zet de status van de metadata op “gepubliceerd”.
3.2 GeoNetwork publiceert de record in de catalogus (met URI).
4.	Beschikbaar stellen DCAT3-M2M via endpoint 
4.1 DCAT Transformer exposeert de catalogus (of subset) via een DCAT AP NL / DCAT3 endpoint, bijv.:
•	catalogus niveau: https://ngr.example.org/dcat-ap-nl
•	per dataset: https://ngr.example.org/datasets/{identifier}?format=dcat-ap-nl
4.2 De vertrouwde dataset is via dit endpoint machine-leesbaar als RDF (JSON LD, Turtle of RDF/XML).
4.3 Externe systemen kunnen deze endpoint URL gebruiken voor automatische harvesting (zie use cases 2, 3, 4).
5.	Beschikbaar stellen DCAT3-H2M via file download 
5.1 NGR biedt (desnoods als extra feature) een functie “Exporteer metadata als DCAT AP NL (RDF)”
5.2 Datapublisher of beheerder:
•	selecteert de dataset,
•	kiest exportformaat (bijv. Turtle of JSON LD),
•	downloadt het bestand (bijv. dataset-x-dcat-ap-nl.ttl)
5.3 Dit bestand kan handmatig worden geüpload in andere systemen (CKAN, IDS). Zie use case 2.1 en 3.1. 
<br/>
*Postcondities*
•	De dataset is gepubliceerd in NGR, gemarkeerd als ‘vertrouwd’;
•	De DCAT AP NL / DCAT3 metadata is:
  •	machine-leesbaar via het DCAT3-endpoint (M2M).
  •	als file downloadbaar (H2M).
<br/>
<br/>

### Use case 2 – Metadata-uitwisseling tussen NGR (GeoNetwork) en Catalogus Circulaire Grondstromen (CKAN) via DCAT3 ###

**Use case variant 2.1 – Via file upload (H2M)**

Een beheerder exporteert DCAT AP NL / DCAT3 metadata uit NGR als bestand, en importeert dit handmatig in CKAN (catalogus Circulaire Grondstromen).
<br/>
*Actorenmodel*
•	Beheerder / datapublisher (mens).
•	NGR (GeoNetwork).
•	Catalogus Circulaire Grondstromen – CKAN + CKANNext DCAT.
<br/>
*Precondities*
•	Use case 1 is technisch mogelijk (export/ download DCAT AP NL-file uit NGR;
•	CKAN ondersteunt import van DCAT AP NL / RDF (via plugin of script);
•	Mapping NGR ↔ CKAN velden is gedefinieerd.
<br/>
*Uitgevoerde stappen*
1.	Selectie vertrouwde dataset(s) in NGR 1.1 Beheerder filtert in NGR op trusted=true / relevante tag.
1.2 Kiest één of meerdere datasets die in CKAN moeten komen.
2.	Exporteren DCAT AP NL / DCAT3-bestand 2.1 Voor elke dataset (of een bundel) genereert NGR een DCAT AP NL RDF-bestand.
2.2 Beheerder downloadt de file(s) naar de eigen werkomgeving.
3.	Inloggen en import in CKAN 3.1 Beheerder logt in op CKAN.
3.2 Start een importfunctie (bijv. CKAN-extensie of script) voor DCAT AP NL.
3.3 Uploadt het DCAT AP NL bestand.
4.	Mapping en aanmaak CKAN-dataset 4.1 CKAN vertaalt RDF/DCAT AP NL naar het interne CKAN-datamodel:
•	dct:title → title
•	dct:description → notes
•	dcat:keyword → tags
•	dct:publisher → CKAN organization
•	dct:license → license_id
•	dcat:distribution → CKAN resources (URL, format).
4.2 De originele NGR URI wordt als extras-veld opgeslagen (bijv. source_catalog=nationaal-georegister, source_uri=…).
5.	Publicatie in Catalogus Circulaire Grondstromen 5.1 CKAN toont de nieuw aangemaakte dataset als onderdeel van de catalogus.
5.2 Gebruikers kunnen doorklikken naar de NGR-bron indien gewenst.
<br/>
*Postcondities* 
•	De metadata uit NGR is in CKAN beschikbaar voor één of meer datasets;
•	Relatie met bron (NGR) is traceerbaar via URI.
<br/>
**Variant 2.2 – Via harvesting DCAT3-endpoint (M2M)**
<br/>
CKAN harvest automatisch DCAT AP NL / DCAT3-metadata van NGR via een endpoint.
<br/>
*Actorenmodel*
•	NGR (GeoNetwork + DCAT Transformer);
•	CKAN Catalogus Circulaire Grondstromen (CKANNext DCAT);
•	CKAN harvester (machineproces).
<br/>
*Precondities*
•	NGR heeft een DCAT AP NL endpoint zoals in use case 1;
•	CKANNext DCAT of een andere harvester kan van dat endpoint lezen;
•	Filtering op ‘vertrouwde’ datasets is mogelijk (bijv. query parameter of inhoudelijke filter op tag/veld).
<br/>
*Uitgevoerde stappen*
1.	Configureren DCAT-harvester in CKAN 1.1 CKAN-beheerder configureert een nieuwe “DCAT AP NL harvester”:
•	Source URL: NGR DCAT endpoint (bijv. https://ngr.example.org/dcat-ap-nl?tag=trusted).
•	Poll-interval (bijv. 1× per dag).
•	Mappingprofiel: NGR → CKAN.
2.	Initiële harvest 2.1 Harvester roept het NGR DCAT endpoint aan.
2.2 Leest alle DCAT AP NL records.
2.3 Past mapping toe (zoals in 2.1 stap 4).
2.4 Maakt datasets in CKAN aan, met verwijzing naar NGR URI.
3.	Periodieke updates 3.1 Harvester draait periodiek.
3.2 Controleert dct:modified of andere versie-/timestamp velden.
3.3 Bij wijzigingen:
•	Past metadata in CKAN aan.
•	Eventuele verwijderde datasets worden gearchiveerd of gemarkeerd conform afspraken.
<br/>
*Postcondities*
•	CKAN heeft een altijd actuele subset van NGR metadata (vertrouwde datasets) via M2M harvesting.
<br/>

## Opgedane bevindingen    {#4041334C}
pm
