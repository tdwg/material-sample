# TDWG MaterialSample Task Group

## Summary of Activities

## Scope

### Charter

While Darwin Core is described as a bag of terms, users do apply additional semantics to it for different application goals, and this needs to be addressed. Developing a model within the limited scope of the properties and direct relationships of MaterialSample to other classes would be an ideal outcome of this group. The scope of any such modeling is expected to include the classes to be defined below and would possibly include the relationships of MaterialSample to _Identification_, _Occurrence_, _Organism_, and _MeasurementOrFact_.

### Outcome

“Seems like we need a Material Core that documents a physical thing that you need an identifier for. Each record represents a preserved specimen/sample with extensions (including maybe an occurrence extension). GBIF is thinking about parsing these types of records by the different types (e.g. a Material Portal, a DNA portal, a Observation portal). We need a richer view of the provenance of each of the record types.”

~ Tim Robertson

Shortly after the task group began meeting we were made aware of upcoming changes at GBIF that would set up a new scheme for physical material. From the 2021-10-13 Material Sample Task Group Meeting:


“John Wieczorek and Tim Robertson working on six different use cases for updating the model - event based model seems to be the one that works for all these use cases [https://gbif.app.box.com/s/7cr98uozrgrs88lz2r0lgt8w5z4yanyw](https://gbif.app.box.com/s/7cr98uozrgrs88lz2r0lgt8w5z4yanyw) “

Although we continued to have lengthy discussions about MaterialSample vs. Organism and how BasisOfRecord functions in the current GBIF use of DarwinCore, in the end we decided it would be best to focus on the core MaterialSample terms. Because new models were being developed, the modeling of relationships of MaterialSample to _Identification_, _Occurrence_, _Organism_, and _MeasurementOrFact_ seemed to overlap with the work being done elsewhere so we also decided to leave that for a future task force to review.


# Goals

### Charter

Our main goal is to enable physical object data sharing as part of the TDWG corpus of standards. The primary deliverable will be revised formal definitions of the terms below with appropriate use case examples following the Darwin Core format, adapted from the original definitions currently provided in Darwin Core. This does not depend upon any other tasks/goals of the Task Group.

* [MaterialSample](https://dwc.tdwg.org/terms/#materialsample) 
* [PreservedSpecimen](https://dwc.tdwg.org/terms/#preservedspecimen) 
* [LivingSpecimen](https://dwc.tdwg.org/terms/#livingspecimen) 
* [FossilSpecimen](https://dwc.tdwg.org/terms/#fossilspecimen) 

**Other deliverables.**

The primary deliverable will be accompanied by a review of the following properties that fall under [Occurrence](https://dwc.tdwg.org/terms/#occurrence), but seem to be properties of one of the above. The task group will make a recommendation for each of these terms as to which class in the Darwin Core standard these properties belong which may also include recommendations for terms being revised, added, disambiguated, or deprecated. Depends upon definitions provided above.

* [catalogNumber](https://dwc.tdwg.org/terms/#dwc:catalogNumber) 
* [Preparations](https://dwc.tdwg.org/terms/#dwc:preparations) 
* [disposition](https://dwc.tdwg.org/terms/#dwc:disposition) 
* [associatedSequences](https://dwc.tdwg.org/terms/#dwc:associatedSequences) 
* [otherCatalogNumbers](https://dwc.tdwg.org/terms/#dwc:otherCatalogNumbers) 
* [BasisOfRecord](https://dwc.tdwg.org/terms/#dwc:basisOfRecord). 

Recommendations will be provided for a revised formal definition as it pertains to materialSample but will not consider other data types.

**Other documentation**

We intend to document the rationale for creating revised definitions, particularly as these revisions promote physical object data sharing. This documentation should enable the relevant communities of practice (e.g., natural history collections managers) to understand the fundamental concepts, avoiding technical jargon wherever possible. Documentation and recommendations may include:

* Use cases and examples
* Suggest new terms if needed (e.g. preservationType)
* Alignments/mappings to related standards, ontologies and vocabularies when possible and desirable


### Outcome


#### Main Goal


##### [MaterialSample](https://dwc.tdwg.org/terms/#materialsample)


#### There was discussion about when a MaterialSample is also an Organism, whether a MaterialSample is also a “specimen” or is specimen a better term, and how MaterialSample should relate to the “specimen” terms in DWC. We discussed some aspects of the definition of materialSample. 

1. Physical object - yes, but it doesn’t need to remain in existence for there to be data about it
2. Represents something larger of interest - 
3. Identifiable, described, curated? 
    1. Identifiable - perhaps eventually, but there are “unidentified” samples awaiting identification
    2. Described - same as above
    3. Curated - leave it out, it is more important that it was recorded
4. Manipulated so as to facilitate measurement, observation - while this may occur, it isn’t required to have a MaterialSample

We suggest a definition revision from

- A physical result of a sampling (or subsampling) event. In biological collections, the material sample is typically collected, and either preserved or destructively processed.

To

- A material entity that represents an entity of interest in whole or in part.

This also resulted in the creation of a new class - MaterialEntity [https://dwc.tdwg.org/terms/#materialentity](https://dwc.tdwg.org/terms/#materialentity) 


<table>
  <tr>
   <td>
    Definition
   </td>
   <td>
    An entity that can be identified, exists for some period of time, and consists in whole or in part of physical matter while it exists.
   </td>
  </tr>
  <tr>
   <td>
    Comments
   </td>
   <td>
    The term is defined at the most general level to admit descriptions of any subtype of material entity within the scope of Darwin Core. In particular, any kind of material sample, preserved specimen, fossil, or exemplar from living collections is intended to be subsumed under this term.
   </td>
  </tr>
</table>


Which allowed for a broader definition of material and postponed the need for the recommendation below:


The remaining terms in the Primary deliverable were discussed in the context of MaterialSample vs “specimen” and it was determined that these terms represent subclasses of MaterialSample.


##### [PreservedSpecimen](https://dwc.tdwg.org/terms/#preservedspecimen) 


##### [LivingSpecimen](https://dwc.tdwg.org/terms/#livingspecimen) 


##### [FossilSpecimen](https://dwc.tdwg.org/terms/#fossilspecimen) 


We suggest that all three terms be deprecated and that they eventually be considered as part of controlled vocabulary for a new term: materialSampleType (see discussion below).


#### Other Deliverables

Recommendations for a revised formal definition as it pertains to materialSample but  not considering other data types.

* [catalogNumber](https://dwc.tdwg.org/terms/#dwc:catalogNumber) 
* [Preparations](https://dwc.tdwg.org/terms/#dwc:preparations) 
* [disposition](https://dwc.tdwg.org/terms/#dwc:disposition) 
* [associatedSequences](https://dwc.tdwg.org/terms/#dwc:associatedSequences) 
* [otherCatalogNumbers](https://dwc.tdwg.org/terms/#dwc:otherCatalogNumbers) 
* [BasisOfRecord](https://dwc.tdwg.org/terms/#dwc:basisOfRecord). 

Definitions for “material” type terms that made reference to any of the material “subclasses” were updated to refer to MaterialEntity in order to encompass all versions of “material”. This included the terms above as well as other references to MaterialSample in term definitions.


## Next Steps

The addition of the MaterialEntity class helped to bring together various versions of “material”, however, the process still seems incomplete and a task group with the specific task of consolidating “material” terms in Darwin Core would be a good next step. As GBIF continues to test a new model of reporting for material, this seems like an excellent time to think about creating a schema for material using the available terms that goes beyond the “bag of terms” currently represented.

In particular, creating a MaterialEntity type term with appropriate vocabulary that could replace the somewhat confusing choices among PreservedSpecimen, LivingSpecimen, FossilSpecimen, and MaterialSample that can currently be used as “basisOfRecord” for data published to an IPT.

Our discussions led us to this, but we felt it was beyond the scope of our task group to push it through:

* materialSampleType
    * Biological 
        * Preserved
        * Living
        * Fossil
        * Tissue
    * Geological
    * Anthropological
    * Environmental
        * Terrestrial
        * Marine
        * Freshwater
        * Atmospheric

