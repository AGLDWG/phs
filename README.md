# Plant Health Surveillance Ontology
RDF documentation of the **Pest Record Specification** (PRS) for *Plant Health Surveillance*.
* During developmemt, view the [latest rendering of the phs ontology](https://raw.githack.com/AGLDWG/phs-ont/master/phs.html) here.

### Vocabularies
This PHS ontology referest to a number of vocabularies which are presented in the [vocabularies/](vocabularies/README.md) folder.

We are currently automating the documentation and publication of the vocabularies. Prototypes are at this [interim address](http://dawe.surroundaustralia.com/). 

## Background
This work is being carried out by the Australian Government Department of Agriculture and Water Resources in collaboration with Biosecurity Agencies of Austlaina states and territories. 

Plant health surveillance is conducted by biosecurity agencies and industry to maintain food quality, prevent the spread of pests and facilitate trade in foodstuffs. The term **Pest Record** is defined in **[ISPM 6](https://www.ippc.int/en/core-activities/standards-setting/ispms/)**. International Standards for Phytosanitary Measures (ISPMs) are standards adopted by the Commission on Phytosanitary Measures (CPM), which is the governing body of the International Plant Protection Convention (IPPC).

The **PRS** builds on a simpler standard, the National Minimum Dataset Specification (NMDS), which defines fewer data elements, and did not use the Resource Description Framework.

## Resource Description Framework (RDF)
* [Formal definition of RDF](https://www.w3.org/TR/rdf11-concepts/)
* [An introduction to RDF](http://www.dlib.org/dlib/may98/miller/05miller.html), which is more readable than the definition above.
* [Another introductory article](https://www.ontotext.com/knowledgehub/fundamentals/what-is-rdf/), with more colour.

## Darwin Core
The **[Darwin Core](https://en.wikipedia.org/wiki/Darwin_Core)** is a set of data elements that describe biological entities. It was created to extend the **[Dublin Core](https://en.wikipedia.org/wiki/Dublin_Core)**, which was created by librarians as a data standard for describing collections. 

* Practical guide to recording data using Darwin Core: [Simple Darwin Core](https://dwc.tdwg.org/simple/)

## The Pest Record Specification
The **PRS** is based on the Darwin Core, but adds terms that describe atttributes of an *observation*, or *collection event*, which is an attempt to detect a
* a **target pest**
* at a given **location**
* at some **time** or **time period**
* following a defined **protocol** that describes how the activity is carried out.

One of the aims of the PRS is to document and define the data elements that must be recorded to create a usable plant health surveillance observation.

Another function of the PRS is to enable the plant health surveillance to define the data quality standards for graph databases such as the **Plant Health Surveillance Data Store**, which aggregates plant health surveillance observations from various sources and allows them to be analysed and reported upon.

## Participation
This is a public repository, released under the Creative Commons Attribution 4.0 International Licence ([CC BY 4.0](https://creativecommons.org/licenses/by/4.0/)). It permits almost any use, subject to providing credit and license notice. 

If you wish to contribute to the development of the Pest Record Specification, you are welcome to clone or fork this repository and submit your work using a pull request. There is a [wealth of tutorials and references](https://duckduckgo.com/?q=best+practice+git+collaboration+pull+request&atb=v141-1&ia=web) on the internet, but this is a [good start](https://www.thinkful.com/learn/github-pull-request-tutorial/). 

## TODO
* Confirm that policy documentation is cleared for public viewing (in this repository)
* Copy policy doco to this repo, either directly into this file (preferred) or other documents.


