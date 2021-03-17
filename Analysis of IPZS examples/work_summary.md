# Work summary

## analysis objective

Verificare la corretta applicazione dello standard Akoma Ntoso v3 e la conformita alla compliance **Level 2 d** previsto dallo stesso standard.

## actions done

Controllati i sequenti requirement:

- [REQ00] XML ben formato e validato da [XSD Akoma Ntoso v3](http://docs.oasis-open.org/legaldocml/akn-core/v1.0/os/part2-specs/schemas/akomantoso30.xsd)

- [REQ01] Verifica Compliance [Level 2 d](http://docs.oasis-open.org/legaldocml/akn-core/v1.0/os/part1-vocabulary/akn-core-v1.0-os-part1-vocabulary.html#_Toc523925095)

    - [REQ01_01] Level 2 uses the document structure and naming convention of URI/IRI (FRBR metadata) and the IDs according to the AKN naming convention as defined in Akoma Ntoso Naming Convention Version 1.0, chapter 4 and 5, or any functionally-equivalent Naming Convention as defined in Akoma Ntoso Naming Convention Version 1.0, section 4.12.

    - [REQ01_02] basic metadata are added

        1. \<identification> con FRBR
        2. \<publication> dove ha senso, considerata la semantica del tag ["The element publication is the metadata container specifying an official publication event for the FRBR expression of the document."](http://docs.oasis-open.org/legaldocml/akn-core/v1.0/os/part2-specs/os-part2-specs_xsd_Element_publication.html), si è assunto la necessità della presenza del tag
        3. I riferimenti normativi corrispondono a tutti gli elementi utilizzando gli attributi href

    - [REQ01_03] normative references are used

        ***??? hypothesis: la condizione 3 di REQ01_02 copre il presente requirement***

    - [REQ01_04] advanced metadata are added

        presenti i tag: \<lifecycle> \<analysis> \<workflow> \<references>

    - [REQ01_05] semantic elements are added

        presenti i tag: 
        \<date> \<time> \<person> \<organization> \<concept> \<object> \<event> \<location> \<process> \<role> \<term> \<quantity> \<def> \<remark> \<recordedTime> \<vote> \<outcome> \<ins> \<del> \<omissis> \<placeholder> \<fillIn> \<decoration> \<docType> \<docTitle> \<docNumber> \<docProponent> \<docDate> \<legislature> \<session> \<shortTitle> \<docAuthority> \<docPurpose> \<docCommittee> \<docIntroducer> \<docStage> \<docStatus> \<docJurisdiction> \<docketNumber> \<courtType> \<neutralCitation> \<party> \<judge> \<lawyer> \<signature> \<opinion> \<argument>


applicando le seguenti azioni:

- [REQ00] validato XML utilizzando feature "Validate with" di oXygen XML Editor 19.1, build 2019121015

## objects analyzed

- [OBJ00] Acts with subsections [010G0043_VIGENZA_20140821_!main.xml](https://raw.githubusercontent.com/vintra73/AnalysisAkomaNtoso/main/Analysis%20of%20IPZS%20examples/Normattiva/Acts%20with%20subsections/010G0043_VIGENZA_20140821_!main.xml) 

## analysis results

|       | REQ00_01 | REQ01_01 | REQ01_02 | REQ01_04 | REQ01_05 |
|-------|----------|----------|----------|----------|----------|
| OBJ00 | OK       | FAULT00  |          |          |          |
| OBJ01 | OK       |          |          |          |          |
| OBJ02 | OK       |          |          |          |          |

Descrizione dei fallimenti:

- [FAULT00]
