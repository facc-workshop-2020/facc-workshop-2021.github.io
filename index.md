---
layout: page
title: Formal Approaches to Certifying Compliance (FACC)
---

An online workshop on applying formal methods tools and techniques to certification and compliance problems. 

FACC will take place 8am-2pm Pacific time on July 19th. FACC will be affiliated to the CAV conference. 

### Registration 

Please register through CAV’s system: [http://i-cav.org/2021/attending/](http://i-cav.org/2021/attending/). To attend FACC, it is only necessary to register as a 'Workshop/Tut. Attendee'. This will be $75 on or before July 9th, and $125 afterwards. 

### Talk schedule

| Time  | Title.                                    | Speaker | 
| ---   | ---                                       | --- |
| 8.00  | Byron Cook / Mike Dodds                   | Opening Remarks | 
| 8.15  | Apostol Vassilev (NIST)                   | [Cybersecurity Assurance or Insurance? Can Formal Methods make the case for cryptographic assurances?](#apostol-vassilev-nist) | 
| 8.45  | Dan Stocker (Coalfire)                    | *TBC* | 
| 9.15  | Richard Paige (McMasters University)      | [Process-Based Assurance of Critical Software-Intensive Systems using WF+](#richard-paige-mcmasters-university) | 
| 9.45  |                                           | **Break, 30 mins** | 
| 10.15 | Ray Richards (DARPA)                      | Rethinking the evaluation of software for certification | 
| 10.45 | Haniel Barbosa (U Federal de Minas Gerais)| Better SMT proofs for certifying compliance | 
| 11.15 | Sazzadur Rahaman (University of Arizona)  | Compliance Disparity Triangle: Impediments for effective compliance certification | 
| 11.45 |                                           | **Break, 30 mins** | 
| 12.15 | Karthik Amrutesh (Amazon Web Services)    | *TBC* | 
| 12.45 | Lucas Wagner (Collins Aerospace)          | Automating Avionics Certification Activities using Formal Methods | 
| 13.15 | Cesare Tinelli (University of Iowa)       | Practical Generation of Proof Certificates for SMT-based Model Checkers | 
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

*Summary:* Cryptography is fundamental for achieving the cybersecurity objectives every person or organization strives for. Cryptography is by far the dominant means for protecting data in transit or at rest. However, cryptography is not immune from exploits due to defects in the implementation of the algorithms and/or the environment in which they execute. When the fundament is shaky and the security assurances promised by cryptography are elusive, what is the public left to do? Buy insurance? Sure, cybersecurity insurance is on the rise, but it is not a panacea. Fortunately, formal methods can tilt the balance of the dilemma between assurance and insurance in favor of the former. Formal methods are the key to eliminating the problems that have plagued cryptographic implementations over time and over a plethora of embodiments: software, hardware, hybrid, etc. In this talk we will look into the potential formal methods have to solve this problem as well as the possibilities they offer for rethinking the traditional methodologies for validating and certifying crypto implementations.

### Richard Paige (McMasters University)

*Title:* Process-Based Assurance of Critical Software-Intensive Systems using WF+

*Abstract:* Assurance for critical software-intensive systems, such as autonomous vehicles or sophisticated medical devices, is of utmost importance, but is often difficult and expensive. Many existing assurance approaches focus on construction of arguments derived from evidence (e.g., data from safety analysis and testing), presented using notations such as GSN. We instead present a model- based approach, WF+, to safety assurance development that is based on modeling processes (e.g., safety processes), data and constraints as three distinct but interrelated workflows. A WF+ model is thus a representation of an argument over integral data and process flows. We present an example illustrating how WF+ works, and how its tools can be used to model parts of safety standards such as ISO 26262. We discuss the benefits of WF+ compared to traditional assurance case notations like GSN. We present ongoing work on the WF+ toolchain as well as its integration with other tools, including spreadsheets (for requirements specification) and Simulink (for analysis data and control flow).
