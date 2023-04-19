## Term change

* Submitter: [Material Sample Task Group](https://www.tdwg.org/community/osr/material-sample/)
* Efficacy Justification (why is this change necessary?): 
* Demand Justification (if the change is semantic in nature, name at least two organizations that independently need this term): Material Sample Task Group, which includes representatives of over 10 organizations and the Global Biodiversity Information Facility (GBIF) because this would be a standardized term for the highest level classification in its developing "Grand Unified Model": "MaterialEntity"
* Stability Justification (what concerns are there that this might affect existing implementations?): 
* Implications for dwciri: namespace (does this change affect a dwciri term version)?: No

Current Term definition: https://dwc.tdwg.org/list/#dwc_[term name here]

Proposed attributes of the new term version (Please put actual changes to be implemented in **bold** and ~strikethrough~):

* Term name (in lowerCamelCase for properties, UpperCamelCase for classes): associatedSequences
* Term label (English, not normative): Associated Sequences
* Organized in Class (e.g., Occurrence, Event, Location, Taxon): **MaterialEntity** ~~Occurrence~~
* Definition of the term (normative): **A list (concatenated and separated) of identifiers (publication, global unique identifier, URI) of genetic sequence information associated with the MaterialEntity.** ~~A list (concatenated and separated) of identifiers (publication, global unique identifier, URI) of genetic sequence information associated with the Occurrence.~~
* Usage comments (recommendations regarding content, etc., not normative): 
* Examples (not normative): http://www.ncbi.nlm.nih.gov/nuccore/U34853.1, http://www.ncbi.nlm.nih.gov/nuccore/GU328060 | http://www.ncbi.nlm.nih.gov/nuccore/AF326093
* Refines (identifier of the broader term this term refines; normative): 
* Replaces (identifier of the existing term that would be deprecated and replaced by this term; normative): None
* ABCD 2.06 (XPATH of the equivalent term in ABCD or EFG; not normative): DataSets/DataSet/Units/Unit/Sequences/Sequence/ID-in-Database + constant
