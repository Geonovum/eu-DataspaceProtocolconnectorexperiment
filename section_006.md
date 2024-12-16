# Gehanteerde begrippen {#770CD133}

In deze sectie worden de kernconcepten, entiteiten en relaties gedefinieerd, die ten grondslag liggen aan een dataspace en het Dataspace Protocol [[IDS-DSP]]. De [DSP terminologie](https://github.com/International-Data-Spaces-Association/ids-specification/blob/main/model/terminology.md) is hieronder vertaald naar het Nederlands. 

**Aanbieder (‘Provider’)**
Een ‘Deelnemer’, die een ‘Dataset’ aanbiedt. 

**Aanbieding (‘Offer’)**
Een aanbieding is het concreet gebruiksbeleid, dat is gekoppeld aan een specifieke ‘Dataset’.

**Beleid (‘Policy’)**
Een reeks regels, taken en verplichtingen die de gebruiksvoorwaarden voor een ‘Dataset’ bepalen. Ook wel ‘gebruiksbeleid’ genoemd.

**Bericht (‘Message’)**
Een instantiatie van een ‘Berrichttype’

**Berichttype (‘Message Type’)**
Een definitie van de structuur van een ‘Bericht’.

**Deelnemer (‘Participant’)** 
Een lid van een dataspace, dat ‘Datasets’ aanbiedt en/of gebruikt.

**Deelnemende Agent (‘Participant Agent’)**
Een technologiesysteem, dat namens een ‘Deelnemer’ bewerkingen uitvoert en een ‘Dataset’ aanbiedt.

**Catalogus (‘Catalog’)**
Een verzameling ‘ Datasets’ en hun ‘Aanbiedingen’, die wordt geadverteerd door een ‘Aanbieder’. 

**Catalogus Protocol (‘Catalog Protocol’)**
Een set van toegestane ‘Berichttypen’ die worden gebruikt om een catalogus te bevragen bij een ‘Catalogus Service’.

**Catalogus Service (‘Catalog Service’)**
De Catalogus Service is een ‘Participant, die een Çatalogus’ toegankelijk maakt voor de ‘Deelnemers’ aan de data space. 

**Connector (‘Connector’ or ‘Data Service’)**
Een ‘Connector’ is ‘Participant’, die een ‘Overeenkomst’ tot stand brengt en het delen van ‘Datasets’ verzorgt en beheert.

**Consument (‘Consumer’)**
Een ‘Consument’ is een ‘Participant’, die toegang vraagt tot een aangeboden ‘Dataset’.

**Contractonderhandelingen (‘Contract Negotiation’)**
Een reeks interacties tussen een ’Aanbieder’ en een ’Consument’, die een ‘Overeenkomst’ tot stand brengen. Het is een instantiatie van de status-machine van een ‘Protocol voor contractonderhandelingen’

**Dataset (‘Dataset’)**
Gegevens of een technische dienst, die door ‘Deelnemers’ kunnen worden gedeeld.

**Dataspace (‘Dataspace’)**
Een reeks technische diensten, die het interoperabel delen van ‘’Datasets’ tussen entiteiten mogelijk maken.

**Dataspace Autoriteit (‘Dataspace Authority’)**
Een ‘Dataspace Autoriteit’ is een entiteit die een ‘Dataspace’ beheert. De vorm en activiteiten van een ‘Dataspace Authoriteit’ vallen niet onder de Dataspace Protocol specificatie.

**Dataspace registratiedienst (‘Dataspace Registration Service or Dataspace Registry’)**
Een technologiesysteem, dat de status van de ‘Deelnemers’in een dataspace bijhoudt. De vorm en mogelijkheden van een ‘Dataspace Registratiedienst’ vallen niet onder de Dataspace Protocol specificatie.

**Identiteit Provider (‘Identity Provider’)**
Een vertrouwd technologiesysteem, dat identiteits-informatie maakt, onderhoudt en beheert voor een ‘Deelnemer’ en de ‘Deelnemende Agent’.

**Overeenkomst (‘Agreement’)**
Een ‘Overeenkomst’ is een concreet ‘Beleid’ gekoppeld aan een specifieke ‘Dataset’, dat is ondertekend door zowel de aanbieder als de consument. Een Overeenkomst is het resultaat van een ‘Contractonderhandeling’ en is gekoppeld aan precies één ‘Dataset’.

**Protocol voor contractonderhandelingen (‘Contract Negotiation Protocol’)**
Een set van toegestane reeksen ‘Berichttypen’, die zijn gedefinieerd als een status-machine.

**Protocol voor transferproces (‘Transfer Process Protocol’)**
Een set toegestane  berichttypereeksen, die zijn gedefinieerd als een status-machine.

**Transferproces (‘Transfer process’)**
Een reeks interacties tussen een Aanbieder en  een Consument die toegang geven tot een Dataset onder de voorwaarden van een Overeenkomst. Het is een instantiatie van de toestandsmachine van een Transfer Process Protocol.

**Verstrekker van inloggegevens (‘Credential Issuer’)**
Een ‘Verstrekker van inloggegevens’ is een vertrouwd technologiesysteem, dat verifieerbare referenties uitgeeft voor een ‘Deelnemers’ en ‘Participanten’.
