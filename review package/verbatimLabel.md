Issue - https://github.com/tdwg/material-sample/issues/40

## Term change

* Submitter: [Material Sample Task Group](https://www.tdwg.org/community/osr/material-sample/)
* Efficacy Justification (why is this change necessary?): Verbatim Label is currently organized in the MaterialSample class. Organizing this term with MaterialEntity will also provide for its use with any existing classes of material things within Darwin Core, as it would be understood that MaterialEntity would be an informal superclass to dwc:MaterialSample, dwc:PreservedSpecimen, dwc:LivingSpecimen, dwc:FossilSpecimen
* Demand Justification (if the change is semantic in nature, name at least two organizations that independently need this term): Material Sample Task Group, which includes representatives of over 10 organizations and the Global Biodiversity Information Facility (GBIF) because this would be a standardized term for the highest level classification in its developing "Grand Unified Model": "MaterialEntity"
* Stability Justification (what concerns are there that this might affect existing implementations?): Usage as currently occurs in Global Biodiversity Information Facility (GBIF) Darwin Core Archives would not be affected by this change. Darwin Core does not include formal class hierarchies, but if we ignore that formality and imagine what the hierarchy would look like for the classes, we have MaterialEntity as the highest for material things. All of the other material-based classes in Darwin Core (dwc:MaterialSample, dwc:PreservedSpecimen, dwc:LivingSpecimen, dwc:FossilSpecimen) might be expected to have verbatim labels. As there are no other classes in between MaterialEntity and those subtypes, verbatimLabel is best organized with MaterialEntity.
* Implications for dwciri: namespace (does this change affect a dwciri term version)?: No

Current Term definition: https://dwc.tdwg.org/list/#dwc_verbatimLabel (note term is in review - https://github.com/tdwg/dwc/issues/32

Proposed attributes of the new term version (Please put actual changes to be implemented in **bold** and ~strikethrough~):

* Term name (in lowerCamelCase for properties, UpperCamelCase for classes): verbatimLabel
* Term label (English, not normative): Verbatim Label
* Organized in Class (e.g., Occurrence, Event, Location, Taxon): **MaterialEntity** ~~MaterialSample~~
* Definition of the term (normative): A serialized encoding intended to represent the literal, i.e., character by character, textual content of a label affixed on, near, or explicitly associated with a material entity, free from interpretation, translation, or transliteration. 
* Usage comments (recommendations regarding content, etc., not normative): The content of this term should include no embellishments, prefixes, headers or other additions made to the text. Abbreviations must not be expanded and supposed misspellings must not be corrected. Lines or breakpoints between blocks of text that could be verified by seeing the original labels or images of them may be used. Examples of material entities include preserved specimens, fossil specimens, and material samples. Best practice is to use UTF-8 for all characters. Best practice is to add comment “verbatimLabel derived from human transcription” in occurrenceRemarks.
* Examples (not normative): 

    i. For a label affixed to a specimen in a vial, the verbatimLabel would contain:

        ILL: Union Co.
        Wolf Lake by Powder Plant
        Bridge. 1 March 1975
        Coll. S. Ketzler, S. Herbert

        Monotoma
        longicollis 4 ♂
        Det TC McElrath 2018

        INHS
        Insect Collection
        456782

    With comment "verbatimLabel derived from human transcription" added in occurrenceRemarks.

    ii. When using Optical Character Recognition (OCR) techniques against an herbarium sheet, the verbatimLabel would contain:

        0 1 2 3 4 5 6 7 8 9 10
        cm copyright reserved
        The New York
        Botanical Garden

        NEW YORK
        BOTANICAL
        GARDEN

        NEW YORK BOTANICAL GARDEN
        ACADEMY OF NATURAL SCIENCES OF PHILADELPHIA
        EXPLORATION OF BERMUDA
        NO. 355
        Cymbalaria Cymbalaria (L.) Wettst
        Roadside wall, The Crawl.
        STEWARDSON BROWN
        }COLLECTORS AUG. 31-SEPT. 20, 1905
        N.L. BRITTON

        NEW YORK BOTANICAL GARDEN
        00499439

    With comment “verbatimLabel derived from unadulterated OCR output” added in occurrenceRemarks.

* Refines (identifier of the broader term this term refines; normative): None
* Replaces (identifier of the existing term that would be deprecated and replaced by this term; normative): None
* ABCD 2.06 (XPATH of the equivalent term in ABCD or EFG; not normative): /Marks/Mark/MarkText
