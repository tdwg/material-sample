Issue - https://github.com/tdwg/material-sample/issues/39

## Term change

* Submitter: [Material Sample Task Group](https://www.tdwg.org/community/osr/material-sample/)
* Efficacy Justification (why is this change necessary?): It would be understood that MaterialEntity would be an informal superclass to `dwc:MaterialSample`, `dwc:PreservedSpecimen`, `dwc:LivingSpecimen`, `dwc:FossilSpecimen`. Examples involving the use of MaterialEntity would be required.
* Demand Justification (if the change is semantic in nature, name at least two organizations that independently need this term): [Material Sample Task Group](https://www.tdwg.org/community/osr/material-sample/), which includes representatives of over 10 organizations.
* Stability Justification (what concerns are there that this might affect existing implementations?): The addition of MaterialEntity as an example for will facilitate usaged by Global Biodiversity Information Facility (GBIF) Darwin Core Archives.
* Implications for dwciri: namespace (does this change affect a dwciri term version)?: No

Current Term definition: https://dwc.tdwg.org/list/#dwc_basisOfRecord

Proposed attributes of the new term version (Please put actual changes to be implemented in **bold** and ~strikethrough~):

* Term name (in lowerCamelCase for properties, UpperCamelCase for classes): basisOfRecord
* Term label (English, not normative): Basis of Record
* Organized in Class (e.g., Occurrence, Event, Location, Taxon): 
* Definition of the term (normative): The specific nature of the data record.
* Usage comments (recommendations regarding content, etc., not normative): Recommended best practice is to use the standard label of one of the Darwin Core classes.
* Examples (not normative): **MaterialEntity,** PreservedSpecimen, FossilSpecimen, LivingSpecimen, MaterialSample, Event, HumanObservation, MachineObservation, Taxon, Occurrence, MaterialCitation
* Refines (identifier of the broader term this term refines; normative): 
* Replaces (identifier of the existing term that would be deprecated and replaced by this term; normative): None
* ABCD 2.06 (XPATH of the equivalent term in ABCD or EFG; not normative): DataSets/DataSet/Units/Unit/RecordBasis
