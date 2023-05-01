Issue - https://github.com/tdwg/material-sample/issues/38

## Term change

* Submitter: [Material Sample Task Group](https://www.tdwg.org/community/osr/material-sample/)
* Efficacy Justification (why is this change necessary?): It would be understood that MaterialEntity would be an informal superclass to `dwc:MaterialSample`, `dwc:PreservedSpecimen`, `dwc:LivingSpecimen`, `dwc:FossilSpecimen`. Examples involving the use of MaterialSample should be expanded to include MaterialEntity.
* Demand Justification (if the change is semantic in nature, name at least two organizations that independently need this term): Material Sample Task Group, which includes representatives of over 10 organizations and the Global Biodiversity Information Facility (GBIF) because this would be a standardized term for the highest level classification in its developing "Grand Unified Model": "MaterialEntity"
* Stability Justification (what concerns are there that this might affect existing implementations?): Usage as currently occurs in Global Biodiversity Information Facility (GBIF) Darwin Core Archives would not be affected by these changes. Darwin Core does not include formal class hierarchies, but if we ignore that formality and imagine what the hierarchy would look like for the classes, we have MaterialEntity as the highest for material things. All of the other material-based classes in Darwin Core (`dwc:MaterialSample`, `dwc:PreservedSpecimen`, `dwc:LivingSpecimen`, `dwc:FossilSpecimen`) might be expected to have references. As there are no other classes in between MaterialEntity and those subtypes, examples including the subtypes should be expanded to include MaterialEntity.
* Implications for dwciri: namespace (does this change affect a dwciri term version)?: No

Current Term definition: https://dwc.tdwg.org/list/#dcterms_references

Proposed attributes of the new term version (Please put actual changes to be implemented in **bold** and ~strikethrough~):

* Term name (in lowerCamelCase for properties, UpperCamelCase for classes): references
* Term label (English, not normative): References
* Organized in Class (e.g., Occurrence, Event, Location, Taxon): Dublin Core terms namespace
* Definition of the term (normative): A related resource that is referenced, cited, or otherwise pointed to by the described resource.
* Usage comments (recommendations regarding content, etc., not normative): From Dublin Core, "This property is intended to be used with non-literal values. This property is an inverse property of Is Referenced By." The intended usage of this term in Darwin Core is to point to the definitive source representation of the resource (e.g.,Taxon, Occurrence, Event in Darwin Core), if one is available. Note that the intended usage of dcterms:bibliographicCitation in Darwin Core, by contrast, is to provide the preferred way to cite the resource itself.
* Examples (not normative): **MaterialEntity example: http://arctos.database.museum/guid/MVZ:Mamm:165861, Taxon example: https://www.catalogueoflife.org/data/taxon/32664** ~~MaterialSample example: http://arctos.database.museum/guid/MVZ:Mamm:165861, Taxon example: https://www.catalogueoflife.org/data/taxon/32664~~
* Refines (identifier of the broader term this term refines; normative): 
* Replaces (identifier of the existing term that would be deprecated and replaced by this term; normative): None
* ABCD 2.06 (XPATH of the equivalent term in ABCD or EFG; not normative): not in ABCD
