# Working Revision
## Term Change
* Submitter: TDWG MaterialSample Task Group
* Efficacy Justification (why is this change necessary?): The current definition includes information that belongs in usage comments or examples and also relies upon an action (sampling) which the Task Group feels is unnecessary. We wanted to provide a simple definition that could be used by many disciplines.
* Demand Justification (if the change is semantic in nature, name at least two organizations that independently need this term): 
* Stability Justification (what concerns are there that this might affect existing implementations?): 
* Implications for dwciri: namespace (does this change affect a dwciri term version)?: Yes

Current Term definition: https://dwc.tdwg.org/list/#dwc_MaterialSample

Proposed attributes of the new term version (Please put actual changes to be implemented in **bold** and ~strikethrough~):

* Term name (in lowerCamelCase for properties, UpperCamelCase for classes): materialSampleID
* Organized in Class (e.g., Occurrence, Event, Location, Taxon): MaterialSample
* Definition of the term (normative): ~An identifier for the MaterialSample (as opposed to a particular digital record of the material sample). In the absence of a persistent global unique identifier, construct one from a combination of identifiers in the record that will most closely make the materialSampleID globally unique.~ **An identifier for a particular instance of dwc:MaterialSample.**
* Usage comments (recommendations regarding content, etc., not normative): ~Recommended best practice is to use a persistent, globally unique identifier.~**Values of dwc:materialSampleID are intended to uniquely and persistently identify a particular material sample (instance of dwc:MaterialSample) within some context. Examples of context include a particular sample collection, an organization, or the worldwide scale. Recommended best practice is to use a persistent, globally unique identifier. The identifier is bound to a physical object (the material sample) as opposed to a particular digital record (representations) of that physical object.**
* Examples (not normative): ~`06809dc5-f143-459a-be1a-6f03e63fc083`~ **`06809dc5-f143-459a-be1a-6f03e63fc083`, doi - https://www.doi.org/, ark - https://arks.org/**
* Refines (identifier of the broader term this term refines; normative): 
* Replaces (identifier of the existing term that would be deprecated and replaced by this term; normative): 
* ABCD 2.06 (XPATH of the equivalent term in ABCD or EFG; not normative): not in ABCD
# Currently Published Version
<table>
	<thead>
		<tr>
			<th colspan="2"><a id="dwc_materialSampleID"></a>Term Name  dwc:materialSampleID</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Term IRI</td>
			<td><a href="http://rs.tdwg.org/dwc/terms/materialSampleID">http://rs.tdwg.org/dwc/terms/materialSampleID</a></td>
		</tr>
		<tr>
			<td>Modified</td>
			<td>2020-10-28</td>
		</tr>
		<tr>
			<td>Term version IRI</td>
			<td><a href="http://rs.tdwg.org/dwc/terms/version/materialSampleID-2020-10-28">http://rs.tdwg.org/dwc/terms/version/materialSampleID-2020-10-28</a></td>
		</tr>
		<tr>
			<td>Label</td>
			<td>Material Sample ID</td>
		</tr>
		<tr>
			<td>Definition</td>
			<td>An identifier for the MaterialSample (as opposed to a particular digital record of the material sample). In the absence of a persistent global unique identifier, construct one from a combination of identifiers in the record that will most closely make the materialSampleID globally unique.</td>
		</tr>
		<tr>
			<td>Notes</td>
			<td>Recommended best practice is to use a persistent, globally unique identifier.</td>
		</tr>
		<tr>
			<td>Examples</td>
			<td>`06809dc5-f143-459a-be1a-6f03e63fc083`</td>
		</tr>
		<tr>
			<td>ABCD equivalence</td>
			<td>not in ABCD</td>
		</tr>
		<tr>
			<td>Type</td>
			<td>Property</td>
		</tr>
		<tr>
			<td>Executive Committee decision</td>
			<td><a href="http://rs.tdwg.org/decisions/decision-2013-10-09_13">http://rs.tdwg.org/decisions/decision-2013-10-09_13</a></td>
		</tr>
	</tbody>
</table>
