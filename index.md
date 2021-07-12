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
| 9.15  | Richard Paige (McMasters University)      | [Process-Based Assurance of Critical Software-Intensive Systems using WF+](#richard-paige-mcmasters-university) | 
| 9.45  |                                           | **Break, 30 mins** | 
| 10.15 | Ray Richards (DARPA)                      | [Rethinking the evaluation of software for certification](#ray-richards-darpa) | 
| 10.45 | Haniel Barbosa (U Federal de Minas Gerais)| [Better SMT proofs for certifying compliance](haniel-barbosa-u-federal-de-minas-gerais) | 
| 11.15 | Sazzadur Rahaman (University of Arizona)  | [Compliance Disparity Triangle: Impediments for effective compliance certification](#sazzadur-rahaman-university-of-arizona) | 
| 11.45 |                                           | **Break, 30 mins** | 
| 12.15 | Karthik Amrutesh (Amazon Web Services)    | *TBC* | 
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


### Richard Paige (McMasters University)

*Title:* Process-Based Assurance of Critical Software-Intensive Systems using WF+

*Abstract:* Assurance for critical software-intensive systems, such as autonomous vehicles or sophisticated medical devices, is of utmost importance, but is often difficult and expensive. Many existing assurance approaches focus on construction of arguments derived from evidence (e.g., data from safety analysis and testing), presented using notations such as GSN. We instead present a model- based approach, WF+, to safety assurance development that is based on modeling processes (e.g., safety processes), data and constraints as three distinct but interrelated workflows. A WF+ model is thus a representation of an argument over integral data and process flows. We present an example illustrating how WF+ works, and how its tools can be used to model parts of safety standards such as ISO 26262. We discuss the benefits of WF+ compared to traditional assurance case notations like GSN. We present ongoing work on the WF+ toolchain as well as its integration with other tools, including spreadsheets (for requirements specification) and Simulink (for analysis data and control flow).

### Ray Richards (DARPA)

*Title:* Rethinking the evaluation of software for certification

*Abstract:* The evaluation of software to determine its fitness for use has changed little over the decades. Evaluations can be superficial checking compliance for policies that are designed to be one-size-fits-all, or heavily focused on indirect measures of the software’s desired qualities. The DARPA Automated Rapid Certification of Software (ARCOS) program is reimagining the evaluation of software. ARCOS is applying data analytics techniques and automated reasoning to make inferences from what is known about software. Assurance case arguments, supported by evidence, are generated to support the software worthiness for use. This talk will discuss some of the motivation and challenges for the ARCOS program and sample some of the emerging technologies.

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

### Sazzadur Rahaman (University of Arizona)

*Title:* Compliance Disparity Triangle: Impediments for effective compliance certification

*Abstract:* In this talk, I will share my experience in studying the PCI DSS certification process for e-commerce websites. I will also discuss the challenges towards enforcing large-scale, industry-wide compliance checking and certification process in the light of PCI DSS. We were the first to systematically measure the security and compliance of the PCI DSS certification process for e-commerce websites. We developed an e-commerce web application testbed, named BuggyCart, with 35 PCI DSS-related vulnerabilities. We used BuggyCart to examine the capability and limitations of PCI scanners and the rigor of the certification process. Our testbed experiments revealed that the vulnerability screening capabilities of some approved scanning vendors (ASV) are inadequate. 5 of the 6 PCI scanners are not compliant with the ASV scanning guidelines. We also built a lightweight PCI scanner named PciCheckerLite, to measure the compliance status of existing e-commerce services. Our measurement on 1,203 e-commerce websites shows that 86% of the websites have at least one type of vulnerability that should disqualify them as non-compliant. We shared our research outcome with the PCI council to help to improve the existing certification process. This work was selected as the finalist of the CSAW'20 Applied Research Competition in 2020.

### Lucas Wagner (Collins Aerospace)

*Title:* Automating Avionics Certification Activities using Formal Methods

*Abstract:* Lucas Wagner is a Principal Research Scientist at Collins Aerospace. He focuses on industrial application of formal methods. Currently, he is leading an initiative to broaden the rollout of SMT-based automatic test generation technology within Collins. This talk will focus on activities within Collins to utilize automated formal reasoning tools to produce certification artifacts. It will describe current efforts, lessons learned and the anticipated need for formal methods tooling in the future.

### Cesare Tinelli (University of Iowa) 

*Title:* Practical Generation of Proof Certificates for SMT-based Model Checkers

*Abstract:* Sophisticated automated analysis tools such as abstract interpreters, model checkers, and other automated verifiers are now included in the production tool chain of safety-critical systems. To be usable in software development processes sanctioned by certifying authorities these tools need to go through a laborious and expensive "qualification" process. One way to reduce the qualification burden is to use analyzers that produce formal certificates as evidence of the correctness of their analysis. This way the qualification requirements can be shifted from highly complex analyzers to much simpler certificate checkers.
We present a twofold technique for generating and verifying analysis certificates in SMT-based model checkers. Certificates are extracted as inductive invariants and reduced to formal proof terms with the help of a proof-producing SMT solver. These certificates are expressed in terms of the internal representation of the input problem by the model checker. The correctness of translation to this representation is addressed separately in a lightweight manner by proving the observational equivalence between the results of two independent translations. The equivalence proof is done by the model checker itself and generates its own proof certificate. Our experimental evaluation shows that, at the price of minimal instrumentation in the model checker, our approach enables an efficient generation and verification of certificates for non-trivial transition systems and properties.
