Issue - https://github.com/tdwg/material-sample/issues/35

# New Term Request

* **Submitter:** TDWG MaterialSample Task Group

## Justifications

* **Efficacy Justification (why is this term necessary?):** The addition of the MaterialEntity class benefits from having a means to identifiy individual instances of MaterialEntities.
* **Demand Justification (name at least two organizations that independently need this term):** [Material Sample Task Group](https://www.tdwg.org/community/osr/material-sample/), which includes representatives of over 10 organizations.
* **Stability Justification (what concerns are there that this might affect existing implementations?):** This would not prevent the use of any existing identifiers of material things within Darwin Core. However, it would be understood that it would be prefereable to use this term in place of dwc:materialSampleID. This proposal does not commit to a definition of the relationship of this term to dwc:materialSampleID, which is expected to be the subject of future discussion.
* **Implications for dwciri: namespace (does this change affect a dwciri term version)?:** None

Proposed attributes of the new term 

* **Term name (in lowerCamelCase for properties, UpperCamelCase for classes):** materialEntityID
* **Organized in Class (e.g., Occurrence, Event, Location, Taxon):** MaterialEntity
* **Definition of the term (normative):** An identifier for a particular instance of a MaterialEntity.
* **Usage comments (recommendations regarding content, etc., not normative):** Values of materialEntityID are intended to uniquely and persistently identify a particular MaterialEntity within some context. Examples of context include a particular sample collection, an organization, or the worldwide scale. Recommended best practice is to use a persistent, globally unique identifier. The identifier is bound to a physical object (the MaterialEntity) as opposed to a particular digital record (representation) of that physical object.
* **Examples (not normative):** `06809dc5-f143-459a-be1a-6f03e63fc083`
* **Refines (identifier of the broader term this term refines; normative):** None
* **Replaces (identifier of the existing term that would be deprecated and replaced by this term; normative):** None
* **ABCD 2.06 (XPATH of the equivalent term in ABCD or EFG; not normative):** Unit/UnitGUID or Unit/UnitID

## See also
* [main discussion thread in Material Sample TG repo](https://github.com/tdwg/material-sample/issues/35)
* [dwc:MaterialEntity new term proposal](https://github.com/tdwg/material-sample/blob/main/review%20package/MaterialEntity.md)
