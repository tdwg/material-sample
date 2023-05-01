Issue https://github.com/tdwg/material-sample/issues/43

# New Term Request

* **Submitter:** TDWG MaterialSample Task Group

## Justifications

* **Efficacy Justification (why is this term necessary?):** The addition of the MaterialEntity class benefits from having a means to remark on individual instances of MaterialEntities.
* **Demand Justification (name at least two organizations that independently need this term):** Material Sample Task Group, which includes representatives of over 10 organizations and the [Global Biodiversity Information Facility (GBIF)](https://www.gbif.org/) because this would be a standardized term for describing individual instances of material things "MaterialEntity" in its developing "[Grand Unified Model](https://www.gbif.org/composition/HjlTr705BctcnaZkcjRJq/data-model-principal-composition)"
* **Stability Justification (what concerns are there that this might affect existing implementations?):** 
* **Implications for dwciri: namespace (does this change affect a dwciri term version)?:** None

Proposed attributes of the new term 

* **Term name (in lowerCamelCase for properties, UpperCamelCase for classes):** materialEntityRemarks
* **Organized in Class (e.g., Occurrence, Event, Location, Taxon):** MaterialEntity
* **Definition of the term (normative):** Comments or notes about the MaterialEntity instance.
* **Usage comments (recommendations regarding content, etc., not normative):** 
* **Examples (not normative):** `found in association with charred remains`, `some original fragments missing`
* **Refines (identifier of the broader term this term refines; normative):** None
* **Replaces (identifier of the existing term that would be deprecated and replaced by this term; normative):** None
* **ABCD 2.06 (XPATH of the equivalent term in ABCD or EFG; not normative):** DataSets/DataSet/Units/Unit/Notes
