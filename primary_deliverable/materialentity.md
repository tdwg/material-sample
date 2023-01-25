# New Term Request

## Justifications

* **Submitter:** Material Sample Task Group

* **Efficacy Justification (why is this term necessary?):** At the present time, Darwin Core does not have a top level class term for describing physical entities. The Material Sample Task Group has been working for over a year to sort out the relationships among existing classes of material things in Darwin Core with the goal of addressing shortcomings in our ability to share information about physical things. This task has been hampered by the shortcomings of the current broadest term for material things: `dwc:MaterialSample`. Because that term requires an aspect of sampling, it conflates the role of the material (to serve as a sample) and the fundamental type of the resource (that it's a material rather than digital or information resource). This complication has hindered the progress of the group, whose work is now at a critical phase with the need to harmonize its work with that of Latimer Core (currently under review). This proposal would improve the situation by creating a top-level term for material entities in the DwC namespace and allow the group to clarify its work by describing the kinds of material things, rather than material samples.
The local name, label, and definition of the proposed top level term intentionally capitalize on the corresponding element (http://purl.obolibrary.org/obo/BFO_0000040) from the Basic Formal Ontology (BFO). This correspondence is intended to enable linking Darwin Core to the conceptual framework offered by BFO which is used as top-level ontology in a number of knowledge representation schemes in the biological and biomedical domain. At the same time, creating the term in the `dwc` namespace rather than importing the corresponding element from BFO enables to independently assert formal semantic relations between both elements as additional semantic layers on top of the base terminology.

* **Demand Justification (name at least two organizations that independently need this term):** Material Sample Task Group, which includes representatives of over 10 organizations, GBIF because this would be a standardized term for the highest level classification in its developing "Grand Unified Model": "Material Entity"

* **Stability Justification (what concerns are there that this might affect existing implementations?):** This would not prevent the use of any existing classes of material things within Darwin Core. However, it would be understood that it would be a superclass to `dwc:MaterialSample`, `dwc:PreservedSpecimen`, `dwc:LivingSpecimen`, `dwc:FossilSpecimen`. Since entailment-generating assertions are no longer included in basic "bag-of-term" metadata, these subclass relations would not be asserted directly by `subClassOf` statements for those other classes, although such assertions could be included in a vocabulary enhancement layered on top of the Darwin Core bag of terms. The relationship of this term to `dwc:Organism` should be the subject of future discussion.
* **Implications for dwciri: namespace (does this change affect a dwciri term version)?:** N/A since this is not a property

## Proposed attributes of the new term
* **Term name (in lowerCamelCase for properties, UpperCamelCase for classes):** dwc:MaterialEntity
* **Term label (English, not normative):** Material Entity
* **Organized in Class (e.g., Occurrence, Event, Location, Taxon):** N/A, it is a class itself
* **Definition of the term (normative):** A `dwc:MaterialEntity` is an identifiable entity that persists, maintaining its identity, through some period of time and consists in part or whole of some portion of matter at any given time of its existence.
* **Usage comments (recommendations regarding content, etc., not normative):** The term is expected to be used to refer to material entities, i.e. entities that consist in part or whole of physical matter. The term is defined at the most general level to admit descriptions of any subtype of material entity within scope of Darwin Core. In particular, samples, preserved specimen, and exemplars from living collections of any kind are intended to be subsumed by this term.
* **Examples (not normative):** a fossil specimen, a herbarium sheet including the plant specimen, any particular part of the plant-derived material affixed to the herbarium sheet, a frozen tissue sample, a water sample, a meteorite fragment, a wolf in a zoo, a pack of wolfs, a molecule of DNA, a deep-frozen DNA sample, a field notebook, a particular paper page from a field notebook
* **Refines (identifier of the broader term this term refines; normative):** None
* **Replaces (identifier of the existing term that would be deprecated and replaced by this term; normative):**
* **ABCD 2.06 (XPATH of the equivalent term in ABCD or EFG; not normative):** None ([Specimen Unit](https://abcd.tdwg.org/terms/#group-SpecimenUnit) when used to denote a class of things appears to be a broadly construed subclass.)

## See also
* [main discussion thread in Material Sample TG repo](https://github.com/tdwg/material-sample/issues/31)
* [dcterms:PhysicalResource NTR](https://github.com/tdwg/dwc/issues/421#)
* [bfo:MaterialEntity](http://purl.obolibrary.org/obo/BFO_0000040)
