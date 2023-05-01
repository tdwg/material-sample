Issue - https://github.com/tdwg/material-sample/issues/41

## Term change

* Submitter: [Material Sample Task Group](https://www.tdwg.org/community/osr/material-sample/)
* Efficacy Justification (why is this change necessary?): It would be understood that MaterialEntity would be an informal superclass to `dwc:MaterialSample`, `dwc:PreservedSpecimen`, `dwc:LivingSpecimen`, `dwc:FossilSpecimen`. Usage and examples involving the use of MaterialSample should be expanded to include MaterialEntity.
* Demand Justification (if the change is semantic in nature, name at least two organizations that independently need this term): Material Sample Task Group, which includes representatives of over 10 organizations and the Global Biodiversity Information Facility (GBIF) because this would be a standardized term for the highest level classification in its developing "Grand Unified Model": "MaterialEntity"
* Stability Justification (what concerns are there that this might affect existing implementations?): Usage as currently occurs in Global Biodiversity Information Facility (GBIF) Darwin Core Archives would not be affected by these changes. Darwin Core does not include formal class hierarchies, but if we ignore that formality and imagine what the hierarchy would look like for the classes, we have MaterialEntity as the highest for material things. All of the other material-based classes in Darwin Core (`dwc:MaterialSample`, `dwc:PreservedSpecimen`, `dwc:LivingSpecimen`, `dwc:FossilSpecimen`) might be expected to have relationships. As there are no other classes in between MaterialEntity and those subtypes, usage and examples including the subtypes should be expanded to include MaterialEntity.
* Implications for dwciri: namespace (does this change affect a dwciri term version)?: No

Current Term definition: https://dwc.tdwg.org/list/#dwc_[term name here]

Proposed attributes of the new term version (Please put actual changes to be implemented in **bold** and ~strikethrough~):

* Term name (in lowerCamelCase for properties, UpperCamelCase for classes): ResourceRelationship
* Term label (English, not normative): Resource Relationship
* Organized in Class (e.g., Occurrence, Event, Location, Taxon): N/A
* Definition of the term (normative): A relationship of one rdfs:Resource (http://www.w3.org/2000/01/rdf-schema#Resource) to another.
* Usage comments (recommendations regarding content, etc., not normative): Resources can be thought of as identifiable records or instances of classes and may include, but need not be limited to dwc:Occurrence, dwc:Organism, **dwc:MaterialEntity**~~dwc:MaterialSample~~, dwc:Event, dwc:Location, dwc:GeologicalContext, dwc:Identification, or dwc:Taxon.
* Examples (not normative): The weight of an organism in grams. An instance of an Organism is the mother of another instance of an Organism. A uniquely identified Occurrence represents the same Occurrence as another uniquely identified Occurrence. A **MaterialEntity**~~MaterialSample~~ is a subsample of another **MaterialEntity**~~MaterialSample~~.
* Refines (identifier of the broader term this term refines; normative): None
* Replaces (identifier of the existing term that would be deprecated and replaced by this term; normative): None
* ABCD 2.06 (XPATH of the equivalent term in ABCD or EFG; not normative): DataSets/DataSet/Units/Unit/Associations
