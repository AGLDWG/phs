# Plant Health Surveillance Ontology
RDF documentation of the **Pest Record Specification** (PRS) for *Plant Health Surveillance*.

## Background
This 

## Resource Description Framework (RDF)
* [Formal definition of RDF]<https://www.w3.org/TR/rdf11-concepts/>
* [An introduction to RDF]<http://www.dlib.org/dlib/may98/miller/05miller.html>, which is more readable than the definition above.
* [Another introductory article]<https://www.ontotext.com/knowledgehub/fundamentals/what-is-rdf/>, with more colour.

## Darwin Core
The **[Darwin Core]<https://en.wikipedia.org/wiki/Darwin_Core>** is a set of data elements that describe biological entities. It was created to extend the **[Dublin Core]<https://en.wikipedia.org/wiki/Dublin_Core>**, which was created by librarians as a data standard for describing collections. 

## The Pest Record Specification
The **PRS** is based on the Darwin Core, but adds terms that describe atttributes of an *observation*, or *collection event*, which is an attempt to detect a
* a **target pest**
* at a given **location**
* at some **time** or **time period**
* following a defined **protocol** that describes how the activity is carried out.

One of the aims of the PRS is to document and define the data elements that must be recorded to create a usable plant health surveillance observation.

Another function of the PRS is to enable the plant health surveillance to define the data quality standards for graph databases such as the **Plant Health Surveillance Data Store**, which aggregates plant health surveillance observations from various sources and allows them to be analysed and reported upon.

## TODO
* Confirm that policy documentation is cleared for public viewing (in this repository)
* Copy policy doco to this repo, either directly into this file (preferred) or other documents.


[Simple Darwin Core]<https://dwc.tdwg.org/simple/>
