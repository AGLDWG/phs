# Profile

This asset is a _profile_ used in conjunction with the Plant Health Surveillance vocabularies stored within the *vocabularies* folder.

### Profile Hierarchy
The main _profile_ hierarchy, as per **Figure 1**, is stored in the file [phs-profile.ttl](../phs-profile.ttl) which is formulated according to PROF. 

The file contains specfic PHS vocabulary profile resources and artifact instances.

# PHS Profile
By *profile*, what is meant here is "A specification that constrains, extends, combines, or provides guidance or explanation about the usage of other specifications." (from [PROF](https://www.w3.org/TR/dx-prof/#definitions)).

This profile is formulated according to the [Profiles Vocabulary](https://www.w3.org/TR/dx-prof/) and provides [Shapes Constraint Language (SHACL)](https://www.w3.org/TR/shacl/) validator files that can be used to determine whether vocabularies conform to this profile.

This profile is hosted online in [Linked Data](https://www.w3.org/standards/semanticweb/data) form using a persistent web address:

* <https://linked.data.gov.au/def/phs/profile>

This is a *profile* of the following vocabularies:

* [Simple Knowledge Organization System (SKOS)](https://www.w3.org/TR/skos-reference/) implemented by [SURROUND Australia](https://surroundaustralia.com) to allow for the validation of vocabularies by specifiying a profile of SKOS which defines what ConceptScheme, Concept and Collection properties and their relative arrangements and facilitating validation according to:
  * SURROUND Australia's business needs and implementation of best practice linked data governance; and
  * Also aligning with Geoscience Australia's requirements of its vocabularies for its business purposes.

* [GeoSPARQL](http://www.opengis.net/doc/IS/geosparql/1.0), [PROV-O](https://www.w3.org/TR/prov-o/), [SSN](https://www.w3.org/TR/vocab-ssn/) and SSN's core ontology [SOSA](https://www.w3.org/ns/sosa/). This PHS profile presents a specification of constraints on the use of classes from the GeoSparql, PROV-O and SOSA, namely:
  * geo:Feature, geo:Geometry;
  * sosa:FeatureOfInterest, sosa:Observation, sosa:ObservableProperty, sosa:Procedure, sosa:Result, sosa:Sample and sosa:Sampler. These constraints are designed to ensure that:  
    * [TODO]




## Profile Resources

### Specification
This profile's _specification_ - the resource that contains the normative rules - is within the file [profile.html](https://github.com/AGLDWG/phs/blob/master/profile.html) and it is able to be viewed online at:

* <https://github.com/AGLDWG/phs/blob/master/profile.html>

** _NOTE: TODO align new profile file name phs-profile when master branch is updated. Simon Opper 27/7/2021_

### Validator
This profile's rules, as defined in the _specification_ are presented for machine validation of RDF vocabularies in the _shapes data graph_ files at [validators/shapes](../validators/shapes) which conform to the [SHACL](https://www.w3.org/TR/shacl/) standard.

A single aggregating SHACL data shapes graph which imports all the phs validators is at [phs_shapes.shapes.ttl](../validators/shapes/phs_shapes.shapes.ttl).

The SHACL data shapes working in conjunction with test instance data located at [instance_data_using_shacl.ttl](../instance-data/instance_data_using_shacl.ttl). This test data is work in progress and supports indicative demo's of validation using profiles.

Tools such as [pySHACL](https://github.com/RDFLib/pySHACL) and the online [SHACL Playground](https://shacl.org/playground/) or [SHACL Play!](https://shacl-play.sparna.fr/play/) can be used with this shape file to validate vocabulary files.

## License  
This code is licensed using the [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) licence. See the [LICENSE file](LICENSE) for the deed. 

Note [Citation](#citation) below for attribution.


## Citation
To cite this profile, please use the following (formulated in [BibTex](http://www.bibtex.org/)):

```
@software{vocpub-profile,
  author = {{SURROUND Australia Pty Ltd}},
  title = {{Vocabulary Publication Profile}},
  version = {1.0},
  date = {2021},
  publisher = {{SURROUND Australia Pty Ltd}},
  url = {https://w3id.org/profile/vocpub}
}
``` 


## Contact
*publisher:*  
![](style/SURROUND-logo-100.png)  
**SURROUND Australia Pty. Ltd.**  
<https://surroundaustralia.com>  

*creator:*  
**Dr Nicholas J. Car**  
*Data Systems Architect*  
SURROUND Australia Pty. Ltd.  
<nicholas.car@surroudaustralia.com>  
<https://orcid.org/0000-0002-8742-7730>
{"mode":"full","isActive":false}

*creator:*  
**Simon J. Opper**  
*Chief Data Scientist*  
SURROUND Australia Pty. Ltd.  
<simon.opper@surroudaustralia.com>  
<https://orcid.org/0000-0003-3932-5614>
{"mode":"full","isActive":false}