# Plant Health Surveillance Profile
This repository describes a `profile`, that is a standard that specialises other standards, for the recording of 'Plant Health Surviellance' data, as managed by the [Department of Agriculture, Fisheries & Forestry (DAFF)](https://www.agriculture.gov.au)'s PHS project.

This profile contains several major items, the content for most of which is in here but some of the content is managed else where but linked to, for example the vocabularies.

This profile is formally defined as [_Profiles Vocabulary_](https://w3c.github.io/dx-prof/prof/) `Profile` and while this repository README file informally describes its content, the profile has formal machine- and human-readable documentation at:

* **<https://linked.data.gov.au/def/phs/profile>**

## Profile Content
This profile contains the following major items:

1. **Profile Declaration**
    * The formal description of this profile
    * <https://linked.data.gov.au/def/phs/profile>
    * Use HTTP requests for RDF data to get the machine-readable form, e.g. `curl -H 'Accept: text/turtle' https://linked.data.gov.au/def/phs/profile`
    * Files: [profile.html](profile.html), [profile.ttl](profile.ttl)
2. **PHS Ontology**
    * The formal system-independent data model for the PHS system
    * <https://linked.data.gov.au/def/phs>
    * Use HTTP requests for RDF data to get the machine-readable form, e.g. `curl -H 'Accept: text/turtle' https://linked.data.gov.au/def/phs`
    * Files: [phs.html](phs.html), [phs.ttl](phs.ttl)
3. **PHS Vocabularies**
    * Code lists used for classifying items defined in the Ontology
    * These are managed in a general-purpose DAWE vocabulary repository: <https://github.com/surroundaustralia/dawe-vocabs/>
    * They are online in the test vocabulary server at <http://dawe.surroundaustralia.com/>
4. **Data Shapes**
    * [Shapes Constraint Language (SHACL)](https://www.w3.org/TR/shacl/) data validators
    * all within the [validators/](validators/) folder
    * these can be used with SHACL tools such as [pySHACL](https://github.com/RDFLib/pySHACL) and [SHACL Playground](https://shacl.org/playground/)

## Background
This work is being carried out by the Australian Government Department of Agriculture and Water Resources in collaboration with Biosecurity Agencies of Austlaina states and territories. 

Plant health surveillance is conducted by biosecurity agencies and industry to maintain food quality, prevent the spread of pests and facilitate trade in foodstuffs. The term **Pest Record** is defined in **[ISPM 6](https://www.ippc.int/en/core-activities/standards-setting/ispms/)**. International Standards for Phytosanitary Measures (ISPMs) are standards adopted by the Commission on Phytosanitary Measures (CPM), which is the governing body of the International Plant Protection Convention (IPPC).

This work builds on a simpler data standard, the National Minimum Dataset Specification (NMDS), which defines fewer data elements, and did not use semantic modelling.

### Resource Description Framework (RDF)
RDF is the fundamental data model used in all of this PHS work due to its ability to formally define all terms used, such as classes, class properties, data type etc. Use of RDF means there's absolutely no abiguity regarding the meaning - semantics - of model elements.

* [Formal definition of RDF](https://www.w3.org/TR/rdf11-concepts/)
* [An introduction to RDF](http://www.dlib.org/dlib/may98/miller/05miller.html), which is more readable than the definition above.
* [Another introductory article](https://www.ontotext.com/knowledgehub/fundamentals/what-is-rdf/), with more colour.

On top of RDF, this system uses the [Web Ontology Language (OWL)](https://www.w3.org/OWL/) as the main modelling system. OWL uses RDF to defin classes, sets of things etc.

### Darwin Core
The **[Darwin Core](https://en.wikipedia.org/wiki/Darwin_Core)** is a set of data elements that describe biological entities. It was created to extend the **[Dublin Core](https://en.wikipedia.org/wiki/Dublin_Core)**, which was created by librarians as a data standard for describing collections. Both Darwin and Dublin Core are implemented in RDF.

* Practical guide to recording data using Darwin Core: [Simple Darwin Core](https://dwc.tdwg.org/simple/)

## This Specification
The ontology defines this formal data model in this profile. In outline, it based on Darwin Core, but adds terms that describe atttributes of an *observation*, or *collection event*, which is an attempt to detect a:

* a **target pest**
* at a given **location**
* at some **time** or **time period**
* following a defined **protocol** that describes how the activity is carried out.

One of the aims of the PHS is to document and define the data elements that must be recorded to create a usable plant health surveillance observation.

Another function of the PHS is to enable the plant health surveillance to define the data quality standards for databases such as the **Plant Health Surveillance Data Store**, which aggregates plant health surveillance observations from various sources and allows them to be analysed and reported upon.

## Participation
This is a public repository which permits almost any use, subject to providing credit and license notice. (see License section next).

If you wish to contribute to this work directly, you are welcome to clone or fork this repository and submit your work using a Pull Request. There is a [wealth of tutorials and references](https://duckduckgo.com/?q=best+practice+git+collaboration+pull+request&atb=v141-1&ia=web) on the internet, but this is a [good start](https://www.thinkful.com/learn/github-pull-request-tutorial/). 

See the Issue Tracker here:

* <https://github.com/AGLDWG/phs/issues>

## License
This profile's content is released under the Creative Commons Attribution 4.0 International Licence ([CC BY 4.0](https://creativecommons.org/licenses/by/4.0/)) and a copy of [the deed](LICENSE) of that license is contained here.

## Citation
To cite this work, as required for on-use, please refer to the profile or the profile elements, such as the ontology, by their persistent web addresses, e.g. <https://linked.data.gov.au/def/phs>. If using a reference manager, consider the following BibTex:

```
@misc{phs_profile_2021,
	title = {Plant Health Surveillance Profile},
	type = {Semantic Web Standard},
	url = {https://linked.data.gov.au/def/phs/profile},
	author = {{Stephen J. Pratt}, {Nicholas J. Car}, {Simon J. Opper}, {Simon J.D. Cox}},
	year = {2021},
}
```

Or just the ontology:

```
@misc{phs_ont_2021,
	title = {Plant Health Surveillance Ontology},
	type = {Semantic Web data model},
	url = {https://linked.data.gov.au/def/phs},
	author = {{Stephen J. Pratt}, {Nicholas J. Car}, {Simon J. Opper}, {Simon J.D. Cox}},
	year = {2021},
}
```

## Contact
This profile was created by DAWE and SURROUND Australia staff. DAWE is the product owner and SURROUND Australia techncially maintains it.

Product Owner:  
**Stephen Pratt**  
_Department of Agriculture, Water and the Environment_  
<stephen.pratt@awe.gov.au>

Technical contact:  
**SURROUND Australia Pty Ltd**  
<https://surroundaustralia.com>  
<info@surroundaustralia.com>  

