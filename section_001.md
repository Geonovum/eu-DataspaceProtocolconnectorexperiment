# Inleiding {#12DAD25F}
Het ministerie van VRO (afdeling Kennis en Geo-informatie) werkt samen met het Beraad voor Geo-informatie aan het programma ‘Zicht op Nederland Datafundament’, waarin wordt gewerkt aan een toekomstvast, flexibel en samenhangend geo-datafundament. Een ander relevant programma is ‘Realisatie IBDS’ (Interbestuurlijke Datastrategie) dat wordt aangestuurd door het Overheidsbreed Beleidsoverleg Digitale Overheid (OBDO) en het Interbestuurlijk Data Overleg (IDO). Een van de projecten van het programma Realisatie IBDS is het Federatief Datastelsel dat gezien wordt als een doorontwikkeling van het huidige stelsel van basisregistraties. Zowel Zicht op Nederland Datafundament als Realisatie IBDS stuurt op het delen van data volgens het ‘data bij de bron’ principe. Data spaces bieden de mogelijkheid om data veilig en vertrouwd uit te wisselen waarbij geen kopieën van de data worden gemaakt (data bij de bron).  
<br/>
<br/> 
Het experiment heeft als doel het IDSA data space protocol en de data connector in de praktijk te testen en opgedane bevindingen en aanbevelingen te beschrijven zodat het experiment herhaalbaar is en anderen ook kennis te laten maken met de werking van het data space protocol. 
## Context experiment: EU data spaces {#5D9FCCAA}
Het concept data space komt voort uit de Europese Datastrategie. De Europese Data Strategie die begin 2020 is voorgesteld, streeft naar een eenheidsmarkt voor de beschikbaarheid en het gebruik van data. De strategie is daarbij gericht op het wereldwijd concurrentievermogen van Europa en op datasoevereiniteit. Technisch wordt naar een pan-Europese data space (dataruimte) gestreefd om te zorgen dat er meer data beschikbaar komt voor socio-economisch gebruik, terwijl bedrijven en individuen die data genereren er wel zeggenschap over blijven houden.  
<br/>
<br/>
Deze pan-Europese data space wordt opgebouwd met meerdere sectorale data spaces die vervolgens onderling interoperabel zijn. Binnen sectoren en thema's zijn er vaak al geldende afspraken t.a.v. standaarden en professionele normen t.a.v. omgang met data, die telkens gebaseerd zijn op de context van die sector. Een data space bouwt daar dan op voort, zowel om dubbel werk te voorkomen als om de vorming van data spaces te versnellen. 
<br/>
<br/>
Zie ook ‘Handreiking EU Informatie m.b.t. digitale en data-strategie' voor het wettelijke kader en ‘Verkenning dataspaces’ voor richtinggevende data space initiatieven in Nederland en Europa en de positie van de Nationale Geo-informatie Infrastructuur (NGII) in deze initiatieven.
<br/>
<br/>
GDDS 
Use case Circulaire grondstromen
## Het experiment {#026C60F0}
Dit experiment is een verkenning naar het gebruiken van het IDSA Dataspace Protocol en data connector in een data-deel experiment binnen de casus Circulaire grondstromen. Het gaat om een praktijk casus waarbij data van een publiek of private partij binnen Circulaire grondstromen vertrouwd en sovereign gedeeld wordt met een derde vragende partij. 
<br/>
<br/>
Binnen het gedachtegoed van data spaces staat het veilig en vertrouwd uitwisselen van data centraal. Het Dataspace Protocol, dat is ontwikkeld door IDSA is hierin gepositioneerd als een  mogelijke voorziene (ISO/IEC) standaard in data spaces om vertrouwd data delen mogelijk te maken.  Om voorbereid te zijn op de toekomst is het doel van deze verkenning een beter beeld te krijgen van de wijze waarop de IDSA Dataspace Protocol connector functioneert in een  minimum viable data space setting. 
<br/>
<br/>
Een belangrijk doel van het experiment voor Geonovum is verder kennismaken met het IDSA Dataspace Protocol en de data connector en te leren in een praktijkcasus hoe deze toe te passen. Daarbij wordt de Dataspace Protocol connector  in een minimal vailable data space setting toegepast bij 2 of 3 use cases uit de praktijk casus Circulaire grondstromen.  
<br/>
<br/>
Het experiment zal daarvoor gebruik maken van een technische experimenteeromgeving van de opdrachtnemer en zal geen operationele omgeving opleveren. Het is een leerexperiment, dat wordt vastgelegd in een rapportage met een onderbouwing van alle gemaakte keuzes, de opgedane bevindingen en aanbevelingen en in online trainingsmateriaal zodat het experiment eenvoudig herhaalbaar is om  anderen ook kennis te laten maken met de werking van het Dataspace Protocol. 
<br/>
<br/>
Om dit doel te bereiken vraagt Geonovum aan de opdrachtnemer: 
<ol><li>Uitwerking van twee of drie use cases (user stories) voor data delen binnen Circulaire grondstromen;</li>
<li>Implementatie van Dataspace Protocol connector en het daadwerkelijk data delen in de twee of drie use cases; </li>
<li>Verslaglegging met aandacht voor de use cases, functionele aspecten van het data delen volgens het MVD concept, de implementatie van de Dataspace Protocol connector (software) en van de opgedane bevindingen in een respec document;</li>
<li>Online trainingsmateriaal zodat het experiment eenvoudig herhaalbaar is.</li>
</ol>
 
De inzet van opdrachtnemer resulteert in:
<ul><li>Rapportage (respec document in de Geonovum omgeving) met uitgevoerde werkzaamheden en opgedane bevindingen en evt. aanbevelingen;</li>
<li>Praktijkworkshop ‘IDS data space connector’ (online trainingsmateriaal);</li>
</ul>
<br/>
<br/>
De rapportage met opgedane bevindingen is een digitaal document en wordt gepubliceerd als respec document op de website van Geonovum.

## Aanpak experiment; minimum viable data space {#38020F80}
Voor de uitvoering van het experiment is de volgende aanpak gehanteerd. Volgens het concept van een ‘minimum viable data space’ is met twee of drie use cases binnen de casus Circulaire grondstromen een experiment uitgevoerd met vertrouwd en souvereign data delen. Daarbij is het open en gestandaardiseerd ‘Dataspace Protocol’ toegepast, dat is geïmplementeerd in diverse data connector software producten. Er is gebruik gemaakt van de TNO Security Gateway (TSG), die als open source software beschikbaar is. Deze <a href='https://internationaldataspaces.org/data-connector-report/' target='_blank'>implementatie van het Dataspace Protocol is gecertificeerd</a> door het IDSA. 
<br/>
<br/>
Een Minimum Viable Data Space (MVDS) is een combinatie van componenten die het mogelijk maken om een data space te creëren met net genoeg functies om bruikbaar te zijn voor veilige en soevereine data-uitwisseling tussen twee partijen, zoals gespecificeerd door de International Data Spaces Association (IDSA). Het doel van een MVDS is om het implementatieproces te stroomlijnen, waardoor het gemakkelijker en sneller wordt om een werkende data space te creëren met veilige en soevereine data-uitwisseling. Door te beginnen met een MVDS kan het ontwikkelteam snel itereren en reageren op de vereisten van de data space, door indien nodig aanpassingen te maken om aan de behoeften van gebruikers te voldoen.
<br/>
<br/>
Het MVDS concept willen we toepassen om het werk van het experiment te vergemakkelijken door de implementatietijd te verkorten (door lange details te vermijden die de eerste release zouden vertragen). Dit stelt ons in staat om te beginnen met een eerste werkende versie (waar veilige en soevereine data-uitwisseling tussen twee partijen wordt toegestaan), waar het ontwikkelteam de aannames over de vereisten van de data space kan herhalen, identificeren en erop kan reageren. 

## Componenten van een MVDS {#6944BD65}
Een MVDS bestaat uit:
1. Twee connectoren (één als dataprovider en één als dataconsument); 
2. Een identiteitsprovider (Dynamic Attribute Provisioning Service, Certificate Authority)
3. Optionele en aanvullende componenten, zoals een metadata makelaar, een app store, een clearinghouse of een vocabulaireprovider, kunnen aan de MVDS worden toegevoegd om de functionaliteit uit te breiden en meer geavanceerde functies mogelijk te maken, zoals het zoeken naar datasets.
<br/>
<br/>
De MVDS biedt een startpunt voor het experiment om een functionele data space te creëren, die naar behoefte kan worden aangepast en uitgebreid om aan specifieke vereisten te voldoen.
<img src='media/image4.png' alt='Minimum Viable Data Space' style='width: 100%;'></img>
<br/>
<br/>
Voor de uitvoering van dit experiment wordt de volgende aanpak voorgesteld. De volgende activiteiten worden uitgevoerd om het Dataspace Protocol experiment uit te voeren: 
<ol><li>Opstellen en ontwerpen use case data delen MVDS concept. Use case i.s.m. Kadaster en CBS. In overleg met Geonovum organiseert opdrachtnemer daarvoor enkele interactieve workshops, zowel vanuit het perspectief van de evt. opgave en data (value case; welke data te delen en waarvoor), welke standaarden worden gebruikt en generieke voorzieningen worden geraadpleegd of uitgevraagd, als ook vanuit rollen en verantwoordelijkheden van de betrokken partijen in het experiment; </li>
<li>Ontwerpen en inrichten van een experimenteeromgeving en evt. bij de deelnemende partijen, zodat alle benodigde technische bouwstenen beschikbaar zijn voor het data-deel experiment;</li>
<li>Uitvoeren data deel experiment tussen de deelnemende partijen. Dat betekent dat de IDSA Dataspace Protocol connectoren worden gevoed met relevante (meta)data, zodat de vertrouwde data-uitwisseling kan worden getest en twee of drie use cases; </li>
<li>De resultaten (bevindingen en aanbevelingen) worden geanalyseerd in enkele workshops en de uitgevoerde data-deel experiment wordt beschreven, de bevindingen en aanbevelingen worden in opstellen;</li>
<li>Opstellen en afstemmen van de rapportage in een respec document; </li>
<li>Presentatie en communicatie van de resultaten in de relevante gremia. <ul><li>Indien nodig zal opdrachtgever een technische experimenteeromgeving (als producer of consumer in een MVDS) beschikbaar stellen voor de opdrachtnemer;</li>
<li>Publicatie van en/of over de eindresultaten van deze opdracht om de kennis en toepassing ervan te bevorderen door communicatie via de Geonovum website en nieuwsbrieven. </li>
</ul>
</li>
</ol>
