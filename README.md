# QoLO

## Quality of Life Ontology

#### See :grey_exclamation: [Issues](https://github.com/sap218/qolo/issues)  for the term-tracker to submit a request (new term/change/suggestion) 

### Creators
* [Samantha Pendleton](https://twitter.com/sap218) Institute of Cancer and Genomic Sciences, University of Birmingham, UK
* [Tasanee Braithwaite](https://twitter.com/tasbraithwaite) The Medical Eye Unit, St Thomas’ Hospital NHS Foundation Trust, London UK
* [Charles ODonovan]() Kings College London, London UK

### Ontology access
* See [LICENSE](https://github.com/sap218/qolo/blob/master/LICENSE) before use 
* See [CHANGELOG](https://github.com/sap218/qolo/blob/master/CHANGELOG.md) before use

### MIRO Guidelines

Below we follow the MIRO guidelines for reporting on an ontology [1]. 

---

**A. The basics**
  * A.1 Quality of Life Ontology (QoLO) - as of 21-09-2021 v0.0.1.
  * A.2 Ontology owner: [Samantha Pendleton](mailto:samanfapc@gmail.com) MSc (Institute of Cancer and Genomic Sciences, University of Birmingham, UK) & [Tasanee Braithwaite](mailto:tasaneebraithwaite@gmail.com) DM (The Medical Eye Unit, St Thomas’ Hospital NHS Foundation Trust, London, UK).
  * A.3 [Licence](https://github.com/sap218/qol/blob/master/LICENSE), which governs the permissions surrounding the ontology, https://creativecommons.org/licenses/by/3.0/.
  * A.4 Named appropriately `qolo.owl`.
  * A.5 Located in GitHub repository: `https://github.com/sap218/qolo`.
  * A.6 Methodological framework: used [Protégé](https://protege.stanford.edu/) software for ontology building.

**B. Motivation**
  * B.1 Ontology is required because on ontology currently exists which meet the Quality of Life domain.
  * B.2 QoLO was developed from domain experts and... (clinical guidelines/literature/patient voice?).
  * B.3 Target audience are those in the research area looking into Quality of Life, plus ophthalmology or extended to other medical domains.

**C. Scope, requirements, development community**
  * C.1 The requirements of the ontology is to be an extensive vocabulary for Quality of Life organised in a condensed, logical, and structured manner. The ontology includes the major Quality of Life domains, therapeutic interventions, and more...
  * C.2 Development community: [Samantha Pendleton](mailto:samanfapc@gmail.com) MSc (Institute of Cancer and Genomic Sciences, University of Birmingham, UK), [Tasanee Braithwaite](mailto:tasaneebraithwaite@gmail.com) DM (The Medical Eye Unit, St Thomas’ Hospital NHS Foundation Trust, London, UK), & [Charles ODonovan](mailto:charles.odonovan@kcl.ac.uk) DM (Kings College London, London, UK)
  * C.3 Issue tracking system used for future developements/requests/bugs: `https://github.com/sap218/qolo/issues`. 

**D. Knowledge acquisition**
  * D.1 Foundation built from clinical guidelines, literature, and experts derived list of terms to be included – and then an extensive review of current biomedical ontologies?
  * D.2 Clinical guidleines and literature included... [citations]. Access to current biomedical ontologies were made via searching ontology repositories, e.g. the [Ontology Lookup Service](https://www.ebi.ac.uk/ols/index).
  * D.3 Experts decided on the contents of QoLO from the sources by... (manual? or was there a different way?)

**E. Ontology content**
  * E.1 Currently (21-09-2021 v0.0.1), ontology format is `RDF/XML OWL` - however ask SP/issues if you wish for an alternative ontology format or advice.
  * E.2 Used [Protégé](https://protege.stanford.edu/) to develop the ontology with Git version control.
  * E.3 Ontology metrics, as of 21-09-2021 version 0.0.1 (see [`CHANGELOG.md`](https://github.com/sap218/qolo/blob/master/CHANGELOG.md)) there are a total of XXX classes, XXX relationships and axioms, XXX annotations, including XXX database cross-references, and XXX patient-preferred synonyms.
  * E.4 Cross-references ontologies inclue: (ontology w/ [citation])
  * E.5 IRI for QoLO is: `https://github.com/sap218/qolo/blob/master/qolo.owl#QOLO_00000`.
  * E.6 Identifier generation policy: Protégé’s preferences schema is that ontology’s entities are to have the prefix “QOL” followed by an underscore then a five digit number: currently they consists of 00001 up to ~00000. All classes have QOL prefix and own numeric identifier since QoLO avoids importing axioms from other ontologies.
  * E.7 Entity metadata policy: currently `exact` synonyms in the ontology are additional clinical/medical terms. However `layperson` synonyms are to be used for all Layman terms...
  * E.8 RO [2] and BFO were used as upper ontologies for relationships.
  * E.9 Currently, relationships in QoLO are cross-referenced, such as `adjacent to` and `treatment of` from RO. We defined our own...based on [citation].
  * E.10 Axiom patterns are inferred from the ontology structure itself (`subclass`) - currently only 100% true cases.

**F. Managing change**
  * F.1 Sustainability plan: QoLO is freely available on GitHub and the creator, Samantha Pendleton, will constantly update/change based on expert opinion or via Issue notifications. Anyone from the community can suggest new terms, but with sufficient evidence/justification, and with support from the development team. Potentially users can `fork` the ontology and make their own changes, which then allows the creator to merge these changes. If often particular individuals are making positive/appropriate changes they can be given direct access to co-maintain the ontology with the creator.
  * F.2 There is the change log ([CHANGELOG.md](https://github.com/sap218/qolo/blob/master/CHANGELOG.md)) for entitles which need to be removed/split/redefined, additionally we can annotate these entities as obsolete. 
  * F.3 Ontology will follow “semantic versioning” guidelines and that it will maintain as version 1 unless a major foundation change is made then it will become version 2. Otherwise additional terms/fixes will increment to version 1.1.0 or 1.0.1 over time. Second digits represent changes to ontology (e.g. multiple class/annotation additions), and third digits represent minor changes (e.g. a few additions).

**G. Quality Assurance**
  * G.1 Successful testing via NLP annotation... on the [Olivia's Vision](http://www.oliviasvision.org/) public forum... Also used Protégé's Pellet reasoner to ensure a coherent and consistent ontology. Experts in the opthamology background deemed/judged the ontology achieves the claims. 
  * G.2 Ontology is novel and first in the Quality of Life domain. QoLO meets the stated requirements as an ontology suitable for clinical use...
  * G.3 An example of application is using the ontology for (sentiment analysis/NLP) on the forum. Additionally future applications include (COGSTACK?)... - QoLO provides an implicit axiomatic structure for data annotated with SNOMED-CT, ICD-10, ICD-9, or Read codes as these are included as cross-references in the ontology, enhancing the potential value of QoLO for searching and curating unstructured clinical data.
  * G.4 Ontology not currently available on other platforms, however future plans indicate availability on biomedical ontology repositories, such as [BioPortal](https://bioportal.bioontology.org/ontologies/).
  * G.5 Current evidence of QoLO application is NLP and sentiment analysis on forum data. To read more, the [manuscript]() will soon be available. We have previously shown that using clinical terms in addition to patient-preferred terms, text mining efforts are increased [3], and so the additional data means more fruitful analsysis to gain a deeper insight of the role online forum play for patients/carers in regards to Quality of Life and Ocular Inflammatory Diseases.

---

[1] Matentzoglu N, Malone J, Mungall C, Stevens R. MIRO: guidelines for minimum information for the reporting of an ontology. Journal of biomedical semantics. 2018 Dec;9(1):1-3.

[2] Smith B, Ceusters W, Klagges B, Köhler J, Kumar A, Lomax J, Mungall C, Neuhaus F, Rector AL, Rosse C. Relations in biomedical ontologies. Genome biology. 2005 May;6(5):1-5.

[3] Pendleton SC, Slater LT, Karwath A, Gilbert RM, Davis N, Pesudovs K, Liu X, Denniston AK, Gkoutos GV, Braithwaite T. Development and application of the ocular immune-mediated inflammatory diseases ontology enhanced with synonyms from online patient support forum conversation. Computers in biology and medicine. 2021 Jun 8:104542.
