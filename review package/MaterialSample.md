Issue - https://github.com/tdwg/material-sample/issues/2

## Term change

* Submitter: [Material Sample Task Group](https://www.tdwg.org/community/osr/material-sample/)
* Efficacy Justification (why is this change necessary?): The MaterialSample Task Group concluded that the adoption of MaterialEntity and the usage comment "In particular, any kind of material sample, .... is intended to be subsumed by this term.", the proposed definition of materialSample should be updated to replace "physical object". 
* Demand Justification (if the change is semantic in nature, name at least two organizations that independently need this term): Material Sample Task Group, which includes representatives of over 10 organizations and the Global Biodiversity Information Facility (GBIF) because this would be a standardized term for the highest level classification in its developing "Grand Unified Model": "MaterialEntity"
* Stability Justification (what concerns are there that this might affect existing implementations?): 
* Implications for dwciri: namespace (does this change affect a dwciri term version)?: No

Current Term definition: https://dwc.tdwg.org/list/#dwc_[term name here]

Proposed attributes of the new term version (Please put actual changes to be implemented in **bold** and ~strikethrough~):

* Term name (in lowerCamelCase for properties, UpperCamelCase for classes): MaterialSample
* Term label (English, not normative): Material Sample
* Organized in Class (e.g., Occurrence, Event, Location, Taxon): N/A
* Definition of the term (normative): **A material entity that represents an entity of interest in whole or in part.** ~~A physical result of a sampling (or subsampling) event. In biological collections, the material sample is typically collected, and either preserved or destructively processed.~~
* Usage comments (recommendations regarding content, etc., not normative): 
* Examples (not normative): A whole organism preserved in a collection. A part of an organism isolated for some purpose. A soil sample. A marine microbial sample.
* Refines (identifier of the broader term this term refines; normative): dwc:MaterialEntity
* Replaces (identifier of the existing term that would be deprecated and replaced by this term; normative): None
* ABCD 2.06 (XPATH of the equivalent term in ABCD or EFG; not normative): DataSets/DataSet/Units/Unit