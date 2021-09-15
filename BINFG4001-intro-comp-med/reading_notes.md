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

