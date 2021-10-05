## Week one 

### Kulikowki-2012 ; Definition of Biomedical informatics 
- theme of the paper is formally defining a set of core philiosphies and high level concepts that make up Biomedical Informatics, and how graduate training should attempt to address/teach them 
#### Intro
- Basically, trying to idnetify core concepts within BMI that can be used for graduate education
#### Definition of BMI
- Scope and breadth of discipline: BMI investigates and supports reasoning, modeling, simulation, experimentation, and translation across the spectrum from molecules to individuals and to populations, from biological to social systems, bridging basic and clinical research and practice and the healthcare enterprise.
- Theory and methodology: BMI develops, studies, and applies theories, methods, and processes for the generation, storage, retrieval, use, management, and sharing of biomed- ical data, information, and knowledge.
- Technological approach: BMI builds on and contributes to computer, telecommunication, and information sciences and technologies, emphasizing their application in biomedicine.
- Human and social context: BMI, recognizing that people are the ultimate users of biomedical information, draws upon the social and behavioral sciences to inform the design and evaluation of technical solutions, policies, and the evolution of economic, ethical, social, educational, and organizational systems.
- and then they basically go through all of these more rigorously, bascially the TLDR is that BMI spans from basic sci to extremley applied, with multiple sub discplines that are all connected by common core concepts, ie BMI{ Health, Bio, Medical, Dental}-informatics
-

#### people in BMI will come form different backgrounds 
- incoming graduate students will not have a well rounded background, but will likely be reasonably experienced in one 3 majors areas - Bio, informatics, or cognitive/social science

### Mitchell-2011, Whats next in Informatics research 
- reviewing the role of informatics in clinical decision support, starting from early beginnings,, moving to current practices, and finishing with future directions 
- DSS == decision support systems 
#### Early clinical decision support methods 
- One of systems used for  small variety of problems. Lack of networking and electronic records, required direct clinician use (60's-80')
- 90's - rapid growth of computing made it seem like DSS would take off, but faced several key challenges
- Domain challenge - Biologt is complicated and hard to understand \
- Systems challenge - the engineering problems of having standardized record keeping, data management, compute resources etc 
- Usage challenge - making something doctors will actually use 
#### current challenges in DSS
- need to make things that are robust, that are able to 
- "there's too much data" - ie how do we provide a way for clinicians to takw advantage of the numerious levels of information that may be available about a patient( EHR, genomic, transcriptomic, environmental, imaging modalities etc)
- accurate genomic medicine will have require large amounts of genomic data, which is challenging in several(obvious) ways;
- we need the right terminology because we need accurate labels for everything 

#### Sweden's  medical terminology - a case study
- used the Snomed-CT terminology standard for clinical care 
- basically, it was a hard process - adoption on all levels is difficult, translation between swedish and english is tricky, etc 
- Moving one level high from this, the standardization of medical terminology across multiple countries, and therefore languages, presents an even greater challenge, but for an equally great payoff

#### Moving forward with DSS
- not just clinicians can benefit from DSS; supporting car workers, hospital admin etc can also use clinical/genomic data to make decisions 
- a tool is only a good tool if it can change outcomes
- admin needs to stop looking to cut costs in the IT dept

## Week two

### Cimmino 1998 - challenges in creating standardized medical terminology
- more of a define the problem paper, rather than talk about specific solutions or implementations 
- currently medical terminology is not working super well, for multiple reasons, some of which are hard to define 
- big problem is lack of expressiveness, ie missing terminology in the vocab corpus
- and so the ability for a vocab system to be able to grow is paramount
- Vocab should be centered around concepts
- This introduces the problems of hierarchy - concepts can be conceputally hierarchical, but individial concepts can be part of multiple hiearchies 
- A semantic graph- nodes are concepts edges are relationships between concepts. relationships are strict verbs, ie "caused by"  "treated by 
- the relational nature of a vocab should allow for differerent levels of granularity
- vocab should also have a context, ie background info from why a specific term was used 
- when a vocab grows, there needs to be a way to tie togehter differnet references of the same concept( ideally in a way that is systamatic, without complete enumeration of all possible references )
- Fig1 - differenty types of conceptual hierarchy 
- Fig2 a semantic graph 
- fig3 example of the same concept evolving across time, haivng both an old way of description and a new way 

## Rector-1999 challenges in creating standardized medical terminology, but again 
- terminology is not meant to be a diagnostic framework, in the sense does not explicitly need to encode inference within the terminology; however, causal relationships will need to be implicitly encoded within the terminology 
- terminology is part of the EHR; use of the terminology use should be seamless, abtracted from in the person inputing the data ; data should be be structured, and queryable  ;terminological data needs to be shared and shared securely across the web;
- terminology can be used to *inform*  decisions on patients, populations, and instituions
- the potential space of medical terminology is enormous - complete enumerations of every scenerio is impossible
- terminology needs to be able to describe clinical concepts(clinical linguistics), be able to be composed to express relationships between concepts(clinical pragmatics), and be interpretable by machines (logical concept representation)
- language carries conceptual baggage that needs to taken into account when designing terminologies 
- as always, the hiearchichal and relational structure of clinical concepts is simply a difficult task 
- terminology needs the ability to incorporate new information, ie synthesize existing concepts into new ones 
- lack of clinical consensus creates an unavoidable variance in terminology usage, with the same concepts being reffered to in different ways
- incorporating existing terminologies - which are an enormous source of data - with new terminologies is also a difficult task 
- key idea: hypothesis of separability: "For a clinical terminology, the representation of concepts and the relations between them can and should be separated from the linguistic knowledge
about how these concepts are expressed in language and the pragmatic knowledge concerning how these concepts are used in dialogues with clinical users."
    - encompases much of what was talked about earlier

## Chute-2005  difficulties of medical terminology, part 3( ;(  )
- Medical terminology, in it current combination of natural language, formal codes, lab tests, EHR etc likely has some sort of latent representation, that is machine readable, but identifying these *de novo* or trying to make one from scratch is very difficult 
- formalization is more useful on the decsion support end, ie between clinicians and a researcher/institution, rather than between clinicians 
- bear in mind all these were written pre-BERT
- equivalency of concepts is also a big problem ie chemical name vs trade name for drugs 
- terminology has varying levels of certainty depending on the patient, ie for a patients just beginning treatment, doctor is not sure what exactly it might be so writes down a ton of stuff
- genomics/transcriptomics may help with the disambiguity of pure language 
- conventional terminology  often has collisons between subspecialties of medcine, 
- ontology vs terminology - ontology is a more rigrous, logic driven conceptual system,  individual concepts are very low-level; terminologies are less formal terminologies, based more on natural language, with individual terms being more descriptive 
- amount of granularity in a system is also another big issue, see above for more reasons why
- While a less granular terminology is easier on the user, a more granular one is better for usbaility
    - Aggregetion logics could be a way to automatically convert highly granular data into 
- there won't ever be a single absolute terminology, so thesauri for translating between terminologies will also be necessary 
 
## Balkyani
- just one pager - TLDR: the phrase "medical concept" is used less in the literature, in favor of semantics and ontology

## Cimino 2005
- the idea of a controlled terminology vs a universal; universal is a generalization about a group of things, or a set of instances in reality
- ie Earth == term, planet that goes around the sun == universal 
- then, by using a combination of universals, we can get more granular on an object ie planets orbiting the Sun AND planets with life == Earth 
- in the medical ontological sense, a universal need not even have a linguistic meaning, but could be inferred or derived from data
- Smith (the proponent of universals ) then proposes that you can chain together universals, over the course of a patient event, to get a unique set of terminolgies specific to a patient 
- argument against universas is that you can encode things that make no sense 
- as as aside, it does kind of feel like these systems are trying to do too much, almost trying to replace the doctor
- universals rely on concepts being static, and would not hold up well to a dynamic concept
- "the purpose of terminologies is to support the recording and use of actual data, rather than primarily as a pure knowledge base of what is known in biomedicine"

## Week 3
Questions for the week

•    **What is an ontology?**
•    **How might ontologies help achieve semantic interoperability?**
•    **Please identify an example of a successful ontology that helps improve the semantic interoperability for a particular domain.**
•    **What roles do ontologies play in biomedical discoveries?**


### Bodenreider-2005 Background on medical terminology
- terminology: controlled set of terms used to describe some field, ie biomedical science
- ontology: the stratification of terminologies into classes, and relationships between these classes 
- there are different classes of ontologies
    - general: not specific to a field(apparently physics can be considered an ontology)
    - domain: specific to a cerrtain field 
    - reference: sharable module of knowledge; can be composed together for formation of new ontologies 
#### Example terminologies
these two are general ontologies, with biomedical sub-groups
- OpenCyc: 1 mil terms, which are divided into groups of microtheories
- WordNet: based on synsets - sets of synonyms for concepts; contains ~114k terms, arranged in a poly-hierarchy 
these ones are ontologies built exclusively for medicine 
- GALEN: re-usable terminology for medical systems; allows terms to be composed together via combination of phenomenons and modifer concepts 
- UMLS: combination of the Metathesaurus, and Semantic network;
    - Metathesaurus: repository of concepts, integrates terms from over 100 sources, over 1mil concepts
    - Semantic network: ontology based on metathesaurus; source agnostic - structures terms within the metathesaurus into 135 semantic types; contains associative relationships
- SNOMED CT: "most comprehensive biomedical terminology" ; have multiple related terms organized into concepts, structuerd in a polyhierarchy; 18 major hierarchies, which can be linked to gether for associative relationships 
- FMA: a general ontology focused on human anatomy, to support the  UMLS; uses two existing general ontologies on physical states and spatial ontologies(3d shpae boundaries, volumes etc) to formaly define huma anatomy
- MENELAS: ontology initally designed for coronary artery disease; organizes terms in concepts, and links them with relational types; makes distinction between real and abstract ideas 

#### Case Study: Blood
Paper goes through an example of how blood is described in different ontologies. 
While all have a roughly similar hierarchy, the major difference is that FMA and SNOMED classify blood as a body subtance, whereas it is a tissue in UMLS and MENELAS; because of these two differences, the functional relationships between blood and other terms is fairly different; TLDR, its hard to align multiple different hierarchies together 

### Joy-01 Designing an ontology

#### Designing an ontology
1. Determine the domain and scop of ontology
    a. Use competency questions - specific task/questions ontology be able to solve - to help define domain and scope
2. If possible, re-use an existing ontology 
3. Identify important terms in the ontology
4. Define the classes and what the organizational hierarchy is; Classes are generally real-world objects/ tangible thing; classes can have attributes aka slots attached to them, A specific instance of a class + its slots can be considered a specific concept
    a. Top down: Start general > get more specific
    b. Bottom up: start specific > collapse into more general terms 
    c. Combination: a+b
5. Define properties of classes(slots)
    a. slots need not be specific to class, many classes can have the same slot, 
6. Define preoperties slots(facets)
    a. Slots can take one or more values; slots can be instances of other classes
    b. Range of slot of type `instance`: all valid classes allowed within the slots
    c. Domain of a slot: all classes that have a specific slot 
7. Create specific instances(these specific instances are concepts )

#### Defining classes and class hierarchy 
- the "is a" relationship generally means that one class is a subclass of anothe, ie if B is_a A  then B \in A; hierarchy is transititve 
- classes should be conceptually atomic; linguistic synonyms should map to the same class
- avoid class cycles
- siblings of a single class should conceptually be similar to each other
- some intermediate classe can be "abstract", and can be marked as such to prevent actual instances of it from being generated
- multiple inheritance -  a class can inherit from two or more parents(this creates a poly-hierarchy )
- disjoint classes: two classes who's set of children do not overlap at all 
- Try not to make class hierarchies too wide or too deep 
- when designing an ontology, when decided whether to make a concept a class or a slot, remember that Ontologies are meant to reflect real-world relationships; for example, in an ontology about wine, should `white_wine` be a distinct class, or should it be `wine(color = 'white')`
- avoid cases where there is a forward and reverse association(slot) between classes; ex: in wine example `Winery produces wine ` and `wine made_by winery` are functionally the same relationship, keep relations flowing in a single direction in the hierarchy 

### Suchman-1994 computer-supported cooperative work(CSCW) 
- bias permeates a system regardless of the creator's intent

### Levesque-1987 Knowledge representations
- The more complicated a terminology is, the harder it is to computationally operate on
- aka hard things are hard 
- knowledge representations are computational representations of natural/physical/semantic knowledge 
    - KRs need to be domain focused 
    - KRs need the ability to express concepts and relationships 

- focuses on the Knowledge base as an example of a KR
- Uses first order logic(FOL) as an example for how a KB can be queried(its kinda confusing tbh), but from what I can tell, you have 
    - non-symbolic ideas that are connected to each other
    - connected ideas can be queried/analyzed by logical symbols, but not sure if connections are themselves logical symbols 
- Basically, the idea is that if you have a KR on a topic, you can *theoretically* use it query specific scenarios 
- this becomes hard because you are essentially going to be making some sort of pseudo - decision tree
    - they call it theorem proving, ie asking a certain relationsip possible -> Y/N
- simplest version of this  would be having data structred in some sort of relational database, that you would then query 
    - but anything you want to query 

## Week 4 
•    **What are the key considerations when evaluating a medical concept representation?**
•    **What are the differences in terminologies and ontologies when representing medical concepts?**
•    **What is the challenge of semantic interoperability?**
•    **What makes medical concept representation difficult?**
•    **Why do we need interface terminologies? What problems were they created to address?**

### Humphreys-1996 Beta Test UMLS
- NLM has a test/contest thingy to get instituions to use the UMLS metathesaurus
- basically a descirption of the availablility of terms and ontologies within the metathesarus 
- basicallly they are telling people to fuck around with the UMLS and find out if its good enough; "crowdsourced auditing" in the context of this weeks material 

### Humphreys-1997 results of the UMLS beta test


### Kanter-2008 EHR in AFrica
-  the standard terminologies of typically ontologies are not in an easily usable format by providers 
- Note that this before the obama era push for EHR adoption 
- Chute's definition of terminology: “that which enables users to invoke a set of controlled terms that correspond to formal concepts organized by a classification schema.”
- Interface terminologies make it easy to use terminology 
- the mapping between interface  terms and refernence terms should ideally be lossless, and  seamless
- they give a good exapmle with asthma - the commonly used description for asthma(in the interface terminology) doest have a snomed term; so map the interface term to a place holder, then change it under the hood once the term becomes available 
- why talk aabout africa? There are many languages spoken, so an optimal solution for implementing a medical terminology system would be to have multiple interface terminologies for the same gold standard reference terminology
- Basically the authors are starting a non-profit to help do what they talked about 

