Issue - https://github.com/tdwg/material-sample/issues/44

## Term change

* Submitter: [Material Sample Task Group](https://www.tdwg.org/community/osr/material-sample/)
* Efficacy Justification (why is this change necessary?): Create consistency of terms for material in Darwin Core.
* Demand Justification (if the change is semantic in nature, name at least two organizations that independently need this term): [Material Sample Task Group](https://www.tdwg.org/community/osr/material-sample/), which includes representatives of over 10 organizations.
* Stability Justification (what concerns are there that this might affect existing implementations?): None
* Implications for dwciri: namespace (does this change affect a dwciri term version)?: No

Current Term definition: https://dwc.tdwg.org/list/#dwc_lithostratigraphicTerms

Proposed attributes of the new term version (Please put actual changes to be implemented in **bold** and ~strikethrough~):

* Term name (in lowerCamelCase for properties, UpperCamelCase for classes): lithostratigraphicTerms
* Term label (English, not normative): Lithostratigraphic Terms
* Organized in Class (e.g., Occurrence, Event, Location, Taxon): Geological Context
* Definition of the term (normative): The combination of all litho-stratigraphic names for the rock from which the ~~cataloged item~~**MaterialEntity** was collected.
* Usage comments (recommendations regarding content, etc., not normative): 
* Examples (not normative): Pleistocene-Weichselien
* Refines (identifier of the broader term this term refines; normative): None
* Replaces (identifier of the existing term that would be deprecated and replaced by this term; normative): None
* ABCD 2.06 (XPATH of the equivalent term in ABCD or EFG; not normative): DataSets/DataSet/Units/Unit/Gathering/Stratigraphy/LithostratigraphicTerms
