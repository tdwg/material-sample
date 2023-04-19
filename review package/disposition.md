## Term change

* Submitter: [Material Sample Task Group](https://www.tdwg.org/community/osr/material-sample/)
* Efficacy Justification (why is this change necessary?): Disposition is currently organized in the Occurrence class. Occurrences are not considered to have dispositions, however the evidence obtained from them do. Organizing this term with MaterialEntity will also provide for its use with any existing classes of material things within Darwin Core, as it would be understood that MaterialEntity would be an informal superclass to `dwc:MaterialSample`, `dwc:PreservedSpecimen`, `dwc:LivingSpecimen`, `dwc:FossilSpecimen`. The examples make clear the intended usage of the term. It is a very specific meaning of the word "disposition" with respect to the availability of an artefact in a collection. The definition change reflects this intent.
* Demand Justification (if the change is semantic in nature, name at least two organizations that independently need this term): Material Sample Task Group, which includes representatives of over 10 organizations and the Global Biodiversity Information Facility (GBIF) because this would be a standardized term for the highest level classification in its developing "Grand Unified Model": "MaterialEntity"
* Stability Justification (what concerns are there that this might affect existing implementations?): Usage as currently occurs in Global Biodiversity Information Facility (GBIF) Darwin Core Archives would not be affected by these changes. Darwin Core does not include formal class hierarchies, but if we ignore that formality and imagine what the hierarchy would look like for the classes, we have MaterialEntity as the highest for material things. All of the other material-based classes in Darwin Core (`dwc:MaterialSample`, `dwc:PreservedSpecimen`, `dwc:LivingSpecimen`, `dwc:FossilSpecimen`) might be expected to have dispositions. As there are no other classes in between MaterialEntity and those subtypes, disposition is best organized with the MaterialEntity.
* Implications for dwciri: namespace (does this change affect a dwciri term version)?: No

Current Term definition: https://dwc.tdwg.org/list/#dwc_[term name here]

Proposed attributes of the new term version (Please put actual changes to be implemented in **bold** and ~strikethrough~):

* Term name (in lowerCamelCase for properties, UpperCamelCase for classes): disposition
* Term label (English, not normative): disposition
* Organized in Class (e.g., Occurrence, Event, Location, Taxon): MaterialEntity
* Definition of the term (normative): **The current state of a MaterialEntity with respect to a collection.** ~~The current state of a specimen with respect to the collection identified in collectionCode or collectionID.~~
* Usage comments (recommendations regarding content, etc., not normative): Recommended best practice is to use a controlled vocabulary.
* Examples (not normative): **in collection, missing, on loan, used up, destroyed, deaccessioned** ~~in collection, missing, voucher elsewhere, duplicates elsewhere~~
* Refines (identifier of the broader term this term refines; normative): 
* Replaces (identifier of the existing term that would be deprecated and replaced by this term; normative): None
* ABCD 2.06 (XPATH of the equivalent term in ABCD or EFG; not normative): DataSets/DataSet/Units/Unit/SpecimenUnit/Disposition
