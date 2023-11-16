# OSLO

## Charter

Het is de bedoeling om een vocabularium en applicatieprofiel uit te werken in lijn met reeds bestaande standaarden (core criterium and evidence vocabularium). Dit applicatieprofiel moet een verlengde vormen van het reeds bestaande ICEG applicatieprofiel Public Service waarvan een implementatieprofiel uitgewerkt is voor de Interbestuurlijke Producten- en Dienstencatalogus (IPDC v3) en de Lokale Producten- en Dienstencatalogus (LPDC).

Rechtenverkenner 2.0 is een eerste toepassing die hiervan gebruik zal maken maar ook andere toepassingen zoals het Verenigingsloket, SDG enz… komen in aanmerking.

Procedure 16c

https://www.vlaanderen.be/digitaal-vlaanderen/agenda/evenementen/oslo-voorwaarden-dienstverlening?order_startdate=asc

Het traject ‘Voorwaarden Dienstverlening’ moet helpen om makkelijk te bepalen of iemand recht heeft of moet voldoen aan een bepaalde publieke dienstverlening.

Dienstverlening kan zowel begrepen worden als een recht (bijvoorbeeld toelage) of een verplichting (bijvoorbeeld belasting). De verstrekkers van deze diensten zijn federale, Vlaamse, provinciale en lokale overheden. Het doel van het OSLO-traject ‘Voorwaarden Dienstverlening’ is het in kaart brengen, definiëren en standaardiseren van informatie met betrekking voorwaarden en bewijsstukken om gebruik te kunnen maken van de dienstverlening.

IPDC: interbestuurlijke producten- en dienstencatalogus

IPDC - LPDC (Implementatiemodel)
https://github.com/Informatievlaanderen/ipdc-lpdc

Use case: beschrijving van de voorwaarden van een PubliekeDienstverlening zodat deze (bij voorkeur automatisch) kunnen worden getoetst.

AP Dienstencataloog
Procedure (CPSV-AP) rule
Criteriumvereiste

OSLO Voorwaarden Dienstverlening
Voorwaarde → Requirement
InformatieConcept → InformationConcept
OndersteundeWaarde → SupportedValue
Bewijs → Evidence
Procedure → Rule

Dieter Van Peer
Heidi Bottu

## OSLO-Steps

https://biblio.ugent.be/publication/01GQEXWF67PEW73F0JHEPYG5VT

https://vlaamseoverheid.sharepoint.com/sites/aiv/tfs/oslo/Shared%20Documents/1.%20Ondersteuning%20%26%20Governance/ICEG

https://poc-procedure.bosa.internetarchitects.be/

https://productencatalogus-v3.vlaanderen.be/nl/instantie/11963




# SEMIC

The Core Criterion and Core Evidence Vocabulary (CCCEV) is designed to support the exchange of information between organisations defining criteria and organisations responding to these criteria by means of evidences.

CCCEV contains two basic and complementary core concepts:
- the Requirement, a broad notion encompassing all forms of requests for information, that is often, but not necessarily, made with the objective to use it as a basis for making a judgement or decision; and
- the Evidence, the data proving or disproving that a specific Requirement is met by someone or something, and thus has been fulfilled.

https://github.com/SEMICeu/cpsv-ap_harvester_federalPilot_Belgium

Requirement: condition or prerequisite that is to be proven by Evidence.

Constraint: Limitation applied to an InformationConcept.  Constraints can be made very precise, namely the limit that must be achieved, is a limit on the value for the associated Information Concept. For example, the InformationConcept would be the age of a person and the Constraint would be the required age in the concext of a specific evaluation.

https://semiceu.github.io/CCCEV/releases/2.00/
InformationConcept
Piece of information that the Evidence or the Requirement needs
InformationConcept: piece of information that the Evidence provides or the Requirement needs. The InformationConcept class offers the ability to describe conceptually the Requirements and provided facts in Evidences. In complementarity with the SupportedValue class, this is a (first) step towards facilitating the assessment of the requirements in an automated way based on the Evidence provided.

InformationConcept::expressionOfExpectedValue
http://data.europa.eu/m8g/expressionOfExpectedValue
Formulation in a formal language of the expected value(s) for the InformationConcept which is aligned with the concepts from the Requirements.
Implementers are free to use their own approach for defining the expected values in more details.

InformationConcept is a tool to make Requirement more machine processable. 

SupportedValue: value for an Information Concept that is provided by an Evidence.
query / value

https://www.youtube.com/watch?v=h4-DqkZ81MQ

https://github.com/SEMICeu/CCCEV/issues/33#issuecomment-1013019145

https://www.youtube.com/watch?v=c04BdKrJuYQ
Mentions SHACL.

# SDG - OOTS

https://ec.europa.eu/digital-building-blocks/wikis/display/TDD/4.1+-+Introduction+to+Exchange+Data+Model+and+Protocol+-+Q1+2023

semantic repository

https://code.europa.eu/oots/tdd/tdd_chapters/-/tree/master/OOTS-EDM

- Evidence Broker
- Data Service Directory
- Semantic Repository

The data model and concepts used in the Evidence Broker are defined in the Core Criterion and Core Evidence Vocabulary (CCCEV, [REF40]), provided by Interoperable Europe [REF29]. Additional design documentation is available for the Evidence Broker [REF9]. 

OASIS RegRep V4 Query Protocol

https://ec.europa.eu/digital-building-blocks/wikis/display/TDD/4.5.1+-+Evidence+Request+Syntax+Mapping+Snapshot+Q2

https://ec.europa.eu/digital-building-blocks/wikis/display/TDD/3.1.3+Information+Data+Model+Snapshot+Q2




# ICEG

Public Service applicatiemodel: Dit model is een toepassingsprofiel van de Core Public Service Vocabulary (CPSV), opgesteld in het kader van de thematische werkgroep van de ICEG, waarin deskundigen van het federale en regionale niveau en van gemeenschappen zijn gegroepeerd

# IPDC-LPDC

De interbestuurlijke producten en dienstencatalogus (IPDC) bevat producten en diensten van overheden in Vlaanderen. Dit zijn producten van zowel bovenlokale als lokale besturen (gevoed door de Lokale Producten en DienstenCatalogus (LPDC)). IPDC tracht zo de centrale bron te zijn voor alle producten en diensten binnen Vlaanderen, en om dit te faciliteren is hij verdeeld in twee delen: concepten en instanties.

# dienst-transactiemodel

https://data.vlaanderen.be/doc/applicatieprofiel/dienst-transactiemodel/


# Datavoorbeelden

https://productencatalogus.vlaanderen.be/fiche/139

huwelijk:
- beschijving voorwaarde minimumleeftijd
- toetsing voorwaarde minimumleeftijd
- resultaat van de toetsing
- bewijs



# RIF

https://lists.w3.org/Archives/Public/public-n3-dev/2021Oct/0012.html

Unless you actually need to query over the constituent parts of the rules, why not store the N3 rules as string literals? You can still connect them to the data to which they apply and get them back with SPARQL queries.

1. translate N3 to RIF
2. store the RIF as RDF

Alternative
:rule1 :appliesTo :Asians ;
  :asN3 "rule 1 expressed in N3 goes here" .

# Implementations

## YourEurope

https://europa.eu/youreurope/search-results/index_en.htm?countryCode=DK&categories=G2

## IPDC - LPDC

https://vlaamseoverheid.atlassian.net/wiki/external/6317081715/ZGU4MGNlODM2N2U1NDU5MGFlY2NlYzcxYmQyYWUwMTc

https://productcatalogus.ipdc.vlaanderen.be/nl/concept/139

https://productcatalogus.ipdc.vlaanderen.be/nl/instantie/36214

# notes

Is it possible to work only with Evidence 
https://informasjonsforvaltning.github.io/cpsv-ap-no/#OversiktOverKlassene

InformationConcept is optional

https://www.itb.ec.europa.eu/shacl/.

De leeftijd van een Agent wordt getoest op timestamp (maakt gebruik van VOC OSLO-Persoon).
```json
{
  "@context": {
    "person": "http://www.w3.org/ns/person#",
    "persoon": "https://data.vlaanderen.be/ns/persoon#",
    "xsd": "http://www.w3.org/2001/XMLSchema#"
  },
  "@type": "person:Person",
  "persoon:Geboorte": {
    "@type": "persoon:Persoonsgebeurtenis",
    "persoon:datum": {
      "@value": "1990-11-08T00:00:00",
      "@type": "xsd:dateTime"
    }
  }
}

```
@prefix sh: <http://www.w3.org/ns/shacl#> .
@prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
@prefix person: <http://www.w3.org/ns/person#> .
@prefix persoon: <https://data.vlaanderen.be/ns/persoon#> .

person:Person
  a sh:NodeShape ;
  sh:targetClass person:Person ;
  sh:property [
    sh:path persoon:Geboorte ;
    sh:property [
      sh:path persoon:datum ;
      sh:datatype xsd:dateTime ;
      sh:maxExclusive "2005-07-26T00:00:00"^^xsd:dateTime ;
    ] ;
  ] .

De leeftijd van een Agent wordt getoest op leeftijd (maakt niet gebruik van VOC OSLO-Persoon).
{
  "@context": {
    "person": "http://www.w3.org/ns/person#",
    "xsd": "http://www.w3.org/2001/XMLSchema#"
  },
  "@type": "person:Person",
  "_:age": {
      "@value": "32",
      "@type": "xsd:integer"
    }
}

@prefix sh: <http://www.w3.org/ns/shacl#> .
@prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
@prefix person: <http://www.w3.org/ns/person#> .

person:Person
    a sh:NodeShape ;
    sh:targetNode _:age ;
    sh:property [
        sh:path xsd:integer ;
        sh:minInclusive 18 ;
    ] .

cccev:InformationConcept
How to express constraints on incoming data?

cccev:SupportedValue
e.g.: how to convert eid authentication into cccev:Agent?
https://ec.europa.eu/digital-building-blocks/wikis/display/TDD/Chapter+2%3A+User+Identification%2C+Authentication+and+Record+Matching+Snapshot+Q2
Specifically, it uses the assured eIDAS user identity attributes obtained from the user authentication in evidence requests.

eidas identifier.

Oplossing voor de OF relatie tussen Voorwaarden.

https://github.com/SEMICeu/CCCEV/issues/51

- Converting public service rules into machine-readable cccev:Requirement

Existing approaches:

1. LOD solution: SHACL

e.g.: [OSLO-steps](https://biblio.ugent.be/publication/01GQEXWF67PEW73F0JHEPYG5VT)

2. non-LOD solution: XML / XSD

e.g.: [OOTS](https://ec.europa.eu/digital-building-blocks/wikis/display/TDD/Latest+version)

- Converting cccev:Evidence into cccev:SupportedValue

For example, how do you go from an eIDAS high identification to a person:Person.
___

Opmerkingen / vragen naar partners die formalisatieoefening zullen doen (textuele beschrijving → gestructureerde procedures):
- Liever een rechtstreekse link cccev:Requirement → cccev:ReferenceFramework of cpsv:PublicService → cpsv:Rule → eli:LegalResource?

Voorstel om een rechstreekse link te voorzien tussen cccev:Requirement → (isDerivedFrom ) eli:LegalResource en eli:LegalResource een subklasse van cccev:ReferenceFramework te maken.

Opmerkingen / vragen naar partners die implementatie van proof of concept zullen doen:
- Het is mogelijk om step:State en sh:NodeShape te encapsuleren in eenzelfde klasse. Hiermee wordt wel een dependency op SHACL vastgelikt. Voordeel is wel dat model eenvoudiger wordt.

Terrasvergunning
https://productencatalogus-v3.vlaanderen.be/nl/concept/768/detail

https://stad.gent/nl/ondernemen/vergunningen-en-regelgeving-voor-ondernemers/horeca/terrassen-gent/vergunning-voor-het-plaatsen-van-een-horecaterras-op-het-openbaar-domein

Horecavergunning
https://productencatalogus-v3.vlaanderen.be/nl/concept/736/detail
https://stad.gent/nl/ondernemen/vergunningen-en-regelgeving-voor-ondernemers/horeca/horeca-attest








