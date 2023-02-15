# materialEntityID
## Associated Github Issues
[materialEntityID](https://github.com/tdwg/material-sample/issues/35)
## Working Revision
### New Term
* Submitter: TDWG MaterialSample Task Group
* Efficacy Justification (why is this term necessary?): The addition of the MaterialEntity class requires a means to identifiy individual MaterialEntities.
* Demand Justification (name at least two organizations that independently need this term): Material Sample Task Group, which includes representatives of over 10 organizations and the [Global Biodiversity Information Facility (GBIF)](https://www.gbif.org/) because this would be a standardized term for describing individual instances of material things "MaterialEntity" in its developing "[Grand Unified Model](https://www.gbif.org/composition/HjlTr705BctcnaZkcjRJq/data-model-principal-composition)"
* Stability Justification (what concerns are there that this might affect existing implementations?): This would not prevent the use of any existing identifiers of material things within Darwin Core. However, it would be understood that it would be prefereable to use this term in place of dwc:materialSampleID. This proposal does not commit to a definition of the relationship of this term to dwc:materialSampleID, which is expected to be the subject of future discussion.
* Implications for dwciri: namespace (does this change affect a dwciri term version)?: No

Proposed attributes of the new term 

* Term name (in lowerCamelCase for properties, UpperCamelCase for classes): materialEntityID
* Organized in Class (e.g., Occurrence, Event, Location, Taxon): MaterialEntity
* Definition of the term (normative): An identifier for a particular instance of dwc:MaterialEntity.
* Usage comments (recommendations regarding content, etc., not normative): Values of dwc:materialEntityID are intended to uniquely and persistently identify a particular material entity (instance of dwc:MaterialEntity) within some context. Examples of context include a particular sample collection, an organization, or the worldwide scale. Recommended best practice is to use a persistent, globally unique identifier. The identifier is bound to a physical object (the material entity) as opposed to a particular digital record (representations) of that physical object.
* Examples (not normative): `06809dc5-f143-459a-be1a-6f03e63fc083`, doi - https://www.doi.org/, ark - https://arks.org/
* Refines (identifier of the broader term this term refines; normative): None
* Replaces (identifier of the existing term that would be deprecated and replaced by this term; normative): None
* ABCD 2.06 (XPATH of the equivalent term in ABCD or EFG; not normative): not in ABCD
