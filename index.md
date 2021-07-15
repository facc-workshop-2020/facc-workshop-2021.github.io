---
layout: page
title: Formal Approaches to Certifying Compliance (FACC)
---

An online workshop on applying formal methods tools and techniques to certification and compliance problems. 

FACC will take place 8am-2pm Pacific time on July 19th. FACC will be affiliated to [Computer Aided Verification (CAV) 2021](http://i-cav.org/2021/). 

### Registration 

Please register through CAV’s system: [http://i-cav.org/2021/attending/](http://i-cav.org/2021/attending/). To attend FACC, it is only necessary to register as a 'Workshop/Tut. Attendee'. This will be $75 on or before July 9th, and $125 afterwards. 

### Talk schedule

All times are [PDT](https://www.timeanddate.com/time/zones/pdt). 

| Time  | Title.                                    | Speaker | 
| ---   | ---                                       | --- |
| 8.00  | Byron Cook / Mike Dodds                   | Opening Remarks | 
| 8.15  | Apostol Vassilev (NIST)                   | [Cybersecurity Assurance or Insurance? Can Formal Methods make the case for cryptographic assurances?](#apostol-vassilev-nist) | 
| 8.45  | Dan Stocker (Coalfire)                    | [Early Experience with Evidence from Formal Methods: An Auditor Perspective](#dan-stocker-coalfire) | 
| 9.15  | Richard Paige (McMaster University)      | [Process-Based Assurance of Critical Software-Intensive Systems using WF+](#richard-paige-mcmasters-university) | 
| 9.45  |                                           | **Break, 30 mins** | 
| 10.15 | Ray Richards (DARPA)                      | [Rethinking the evaluation of software for certification](#ray-richards-darpa) | 
| 10.45 | Haniel Barbosa (U Federal de Minas Gerais)| [Better SMT proofs for certifying compliance](haniel-barbosa-u-federal-de-minas-gerais) | 
| 11.15 | Sazzadur Rahaman (University of Arizona)  | [Compliance Disparity Triangle: Impediments for effective compliance certification](#sazzadur-rahaman-university-of-arizona) | 
| 11.45 |                                           | **Break, 30 mins** | 
| 12.15 | Karthik Amrutesh (Amazon Web Services), in conversation with Byron Cook | [How I learned to stop worrying and start applying automated reasoning](#karthik-amrutesh-amazon-web-services) | 
| 12.45 | Lucas Wagner (Collins Aerospace)          | [Automating Avionics Certification Activities using Formal Methods](#lucas-wagner-collins-aerospace) | 
| 13.15 | Cesare Tinelli (University of Iowa)       | [Practical Generation of Proof Certificates for SMT-based Model Checkers](#cesare-tinelli-university-of-iowa) | 
| 13.45 | Byron Cook / Mike Dodds                   | Closing Remarks | 


### Topic 

Regulatory compliance is a requirement for many types of software systems. For example, cryptographic systems may be subject to FIPS certifications, medical data systems must be HIPAA compliant, safety critical systems must adhere to standards such as ISO 26262 and DO-178C, and cloud services used by the US government must achieve FedRAMP designation. Even after software is built and certified, changes to the software, no matter how minor, must often be recertified to ensure that they do not break previously-held assumptions.

Unfortunately, current approaches to compliance can be slow-moving and expensive. This pace directly clashes with modern software development, which is characterized by rapid change and enormous scale. For many organizations compliance imposes unacceptable cost and delay when shipping industry-strength software. In addition, compliance can perversely result in less reliable software, as bug fixes are delayed by certification processes. 

Formal methods may offer solutions to this problem. We seek formal methods tools, solutions, capabilities, or techniques that can be inserted into certification processes to make them cheaper, faster, and more rigorous. 

The FACC workshop will explore how formal methods tools and techniques can increase automation in compliance processes, and thereby help build software more cheaply and reliably. Our aim is to bring together industry, government, and academic experts to share ideas, scope problems, and develop future collaborations.

Topics of interest: 

* Test synthesis
* Formal verification techniques
* Enforcement of security controls
* Detecting and analyzing changes
* Automatically invalidating and regenerating evidence
* Case studies and experience reports

### Co-chairs

* [Mike Dodds](https://galois.com/team/mike-dodds/) (Galois, Inc)
* [Byron Cook](http://www0.cs.ucl.ac.uk/staff/b.cook/) (Amazon Web Services, University College London)

Please direct all inquiries to [Mike Dodds](mailto:miked@galois.com). 

## Talk Abstracts: 

### Apostol Vassilev (NIST)

*Title:* Cybersecurity Assurance or Insurance? Can Formal Methods make the case for cryptographic assurances?

*Abstract:* Cryptography is fundamental for achieving the cybersecurity objectives every person or organization strives for. Cryptography is by far the dominant means for protecting data in transit or at rest. However, cryptography is not immune from exploits due to defects in the implementation of the algorithms and/or the environment in which they execute. When the fundament is shaky and the security assurances promised by cryptography are elusive, what is the public left to do? Buy insurance? Sure, cybersecurity insurance is on the rise, but it is not a panacea. Fortunately, formal methods can tilt the balance of the dilemma between assurance and insurance in favor of the former. Formal methods are the key to eliminating the problems that have plagued cryptographic implementations over time and over a plethora of embodiments: software, hardware, hybrid, etc. In this talk we will look into the potential formal methods have to solve this problem as well as the possibilities they offer for rethinking the traditional methodologies for validating and certifying crypto implementations.

### Dan Stocker (Coalfire)

*Title:* Early Experience with Evidence from Formal Methods: An Auditor Perspective

*Abstract:* Use of formal methods to support audits requires a greater degree of collaboration between auditor and auditee. Our experience has identified key areas where the usual conventions of audit must evolve to support use of evidence adduced from formal methods. Characterizing and categorizing these will help organizations plan for these challenges.

*Bio:* Dan oversees the Payments Advisory Practice at Coalfire, which includes workshops, fit-for-purpose reviews/whitepapers, gap analyses, and larger customer support efforts (remediation and staff augmentation).

In 2018, Dan established the Cloud Advisory practice at Coalfire, which grew out of his work advising and assessing the major cloud service providers (AWS, Azure, Google, Salesforce, IBM and Oracle). Methodology developed in that work has been applied to multiple verticals and to extend security and privacy compliance understanding to leading-edge cloud technology (e.g., containers).
Large financial firms have built private clouds with this guidance. Recent work has focused on coordinated advisory and assessment efforts, combining PCI with GDPR, HITRUST, and FedRAMP.

Dan came to Coalfire from a long career on Wall Street and in the telecommunications industry. In his 11 years at Goldman Sachs, he held lead technical positions in Trading Technology and Tech Risk, including Business Continuity. At AT&T, Dan was a principal SME at the worldwide Frame Relay NOC.


### Richard Paige (McMasters University)

*Title:* Process-Based Assurance of Critical Software-Intensive Systems using WF+

*Abstract:* Assurance for critical software-intensive systems, such as autonomous vehicles or sophisticated medical devices, is of utmost importance, but is often difficult and expensive. Many existing assurance approaches focus on construction of arguments derived from evidence (e.g., data from safety analysis and testing), presented using notations such as GSN. We instead present a model- based approach, WF+, to safety assurance development that is based on modeling processes (e.g., safety processes), data and constraints as three distinct but interrelated workflows. A WF+ model is thus a representation of an argument over integral data and process flows. We present an example illustrating how WF+ works, and how its tools can be used to model parts of safety standards such as ISO 26262. We discuss the benefits of WF+ compared to traditional assurance case notations like GSN. We present ongoing work on the WF+ toolchain as well as its integration with other tools, including spreadsheets (for requirements specification) and Simulink (for analysis data and control flow).

### Ray Richards (DARPA)

*Title:* Rethinking the evaluation of software for certification

*Abstract:* The evaluation of software to determine its fitness for use has changed little over the decades. Evaluations can be superficial checking compliance for policies that are designed to be one-size-fits-all, or heavily focused on indirect measures of the software’s desired qualities. The DARPA Automated Rapid Certification of Software (ARCOS) program is reimagining the evaluation of software. ARCOS is applying data analytics techniques and automated reasoning to make inferences from what is known about software. Assurance case arguments, supported by evidence, are generated to support the software worthiness for use. This talk will discuss some of the motivation and challenges for the ARCOS program and sample some of the emerging technologies.

*Bio:* Dr. Raymond (“Ray”) Richards joined DARPA in January 2016, where he is currently a Program Manager in the Information Innovation Office (I2O).  His research interests focus on high assurance software and systems. While at DARPA he directed the HACMS and VET programs to successful conclusions, and is currently managing the CASE, ARCOS, and IDAS programs. As part of his responsibilities at DARPA, he mentored an honoree of DARPA’s Young Faculty Award, and will be mentoring a recipient of I2O’s recently announced Post-Doctoral Fellowship.

Dr. Richards joined DARPA from Rockwell Collins Advanced Technology Center (ATC) where he led a research group focused on automated analysis, cyber, and information assurance.  In this role he helped to foster the industrial use of formal methods verification to support security accreditations. Under his leadership, two research groups were combined into a single entity, one group focused on cyber and information assurance, the other on formal analysis. The new group was able to leverage their combined strengths and engage in strategic teaming relationships to garner ATC-leading amounts of government funded research contracts. He lead successful collaborative relationships with key academic and industrial partners, fostering collaborative relationships between Rockwell Collins and academic partners that flourish to this day. These partners included Iowa State University, Kansas State University, the University of Illinois, the University of Iowa, the University of Kansas, and the University of Minnesota. Dr. Richards pushed Rockwell Collins’ to support an informal academic workshop called Midwest Verification Day, in which all of the previously named institutions where regular participants. His final role at Rockwell Collins was to serve as the liaison to U.S. Government S&T funding agencies. 

Before assuming a leadership role at Rockwell Collins, he performed research in the formal modeling and analysis of high assurance systems. Often this ground-breaking work was performed in support of practical goals, such as garnering U.S. Government certification of the system that was formally modeled and verified. He led the software development for a high-assurance cross-domain guard, and the formal modeling and analysis effort of a real-time operating system, in support of a Common Criteria EAL6+ evaluation. With over 20 years of experience in leading the development of state-of-the-art computer hardware, software and systems, Dr. Richards has developed real-time software ranging from high fidelity ground vehicle simulators, to safety critical software for air transport aircraft. 

Dr. Richards holds an MBA degree, Ph.D. and M.S. degrees in Electrical and Computer Engineering, and a B.S. degree in Electrical Engineering, all from the University of Iowa. He lives in Northern Virginia with his wife, Lorna. She is in a leadership position at an international Clinical Research Organization. They have two grown children, one in Seattle, and the other in Phoenix. Dr. Richards holds a private pilot’s license and he has logged 12 skydives. His personal interests include running, reading, genealogy, Iowa Hawkeyes sports, and motorcycling.


### Haniel Barbosa (U Federal de Minas Gerais)

*Title:* Better SMT proofs for certifying compliance

*Abstract:* 
SMT solvers can be hard to trust, since it generally means assuming
their large and complex codebases do not contain bugs that lead to
wrong results. Machine-checkable certificates, via proofs of the
logical reasoning the solver has performed, address this issue by
decoupling confidence in the results from the solver's implementation.

Despite previous work, in several SMT solvers, to produce and check
proofs, users still have to choose among solvers that may not produce
fine-grained proofs, may not produce proofs for some of their
crucial-for-efficiency components, or have proofs that are checkable
only as part of a specific proof assistant.

To facilitate the use of SMT proof certificates, the cvc5 developers
team has completely redesigned its proof-production infrastructure,
aiming for a sufficiently general and extensible infrastructure to
allow: the generation of coarse- and fine-grained proofs for all parts
of the solver, particularly for previously unsupported components such
as the rewriter and the strings subsolver; and the printing of proofs
in different formats to enable the use of different proof checkers.
Specifically, we are working on producing cvc5 proofs for LFSC,
Isabelle/HOL, Lean4, and Coq, while also creating proof calculi for
previously unsupported SMT-LIB theories in these settings. While the
project is still ongoing, we will report on significant progress on
all of these fronts.

### Karthik Amrutesh (Amazon Web Services) 

*Title:* How I learned to stop worrying and start applying automated reasoning

*Abstract:* Automated reasoning has real world audit applications beyond the abstract. In this talk, we will share our experience of having applied automated reasoning principles to satisfy auditor expectations on a subset of PCI-DSS (Payment Card Industry – Data Security Standards) requirements. We will discuss our approach to the pilot initiative, lessons learned and the path forward.

*Bio:* Karthik Amrutesh is a senior manager in Security Assurance at AWS. His team is focused on security and privacy audit and attestation activities in Europe, Africa, Latin America and Canada. Prior to joining AWS in October 2020, he had stints as the head of risk and information security at Betterment, a senior manager in the technology risk and assurance practice at Ernst & Young, and an information security advisor at Wipro Consulting.

### Sazzadur Rahaman (University of Arizona)

*Title:* Compliance Disparity Triangle: Impediments for effective compliance certification

*Abstract:* In this talk, I will share my experience in studying the PCI DSS certification process for e-commerce websites. I will also discuss the challenges towards enforcing large-scale, industry-wide compliance checking and certification process in the light of PCI DSS. We were the first to systematically measure the security and compliance of the PCI DSS certification process for e-commerce websites. We developed an e-commerce web application testbed, named BuggyCart, with 35 PCI DSS-related vulnerabilities. We used BuggyCart to examine the capability and limitations of PCI scanners and the rigor of the certification process. Our testbed experiments revealed that the vulnerability screening capabilities of some approved scanning vendors (ASV) are inadequate. 5 of the 6 PCI scanners are not compliant with the ASV scanning guidelines. We also built a lightweight PCI scanner named PciCheckerLite, to measure the compliance status of existing e-commerce services. Our measurement on 1,203 e-commerce websites shows that 86% of the websites have at least one type of vulnerability that should disqualify them as non-compliant. We shared our research outcome with the PCI council to help to improve the existing certification process. This work was selected as the finalist of the CSAW'20 Applied Research Competition in 2020.

*Bio:* Sazzadur Rahaman is an assistant professor in the Department of Computer Science at the University of Arizona. He works towards making security research more democratized and affordable. He is broadly interested in computer security and privacy problems, specifically in building robust systems and methodologies by using program analysis, formal verification, applied cryptography, and machine learning-based techniques. His research stirred both industry and academic interests, over the years. Sazzadur completed his Ph.D. from Virginia Tech. As the recognition of his work, he received several fellowships (Bitshare fellowship and Pratt fellowship) and awards (Torgesen award, CSAW'20 Best paper finalist) at Virginia Tech.

### Lucas Wagner (Collins Aerospace)

*Title:* Automating Avionics Certification Activities using Formal Methods

*Abstract:* Lucas Wagner is a Principal Research Scientist at Collins Aerospace. He focuses on industrial application of formal methods. Currently, he is leading an initiative to broaden the rollout of SMT-based automatic test generation technology within Collins. This talk will focus on activities within Collins to utilize automated formal reasoning tools to produce certification artifacts. It will describe current efforts, lessons learned and the anticipated need for formal methods tooling in the future.

### Cesare Tinelli (University of Iowa) 

*Title:* Practical Generation of Proof Certificates for SMT-based Model Checkers

*Abstract:* Sophisticated automated analysis tools such as abstract interpreters, model checkers, and other automated verifiers are now included in the production tool chain of safety-critical systems. To be usable in software development processes sanctioned by certifying authorities these tools need to go through a laborious and expensive "qualification" process. One way to reduce the qualification burden is to use analyzers that produce formal certificates as evidence of the correctness of their analysis. This way the qualification requirements can be shifted from highly complex analyzers to much simpler certificate checkers.
We present a twofold technique for generating and verifying analysis certificates in SMT-based model checkers. Certificates are extracted as inductive invariants and reduced to formal proof terms with the help of a proof-producing SMT solver. These certificates are expressed in terms of the internal representation of the input problem by the model checker. The correctness of translation to this representation is addressed separately in a lightweight manner by proving the observational equivalence between the results of two independent translations. The equivalence proof is done by the model checker itself and generates its own proof certificate. Our experimental evaluation shows that, at the price of minimal instrumentation in the model checker, our approach enables an efficient generation and verification of certificates for non-trivial transition systems and properties.
