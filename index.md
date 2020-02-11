---
layout: page
title: Formal Approaches to Certifying Compliance (FACC)
---

A workshop on applying formal methods tools and techniques to certification and compliance problems. 

FACC will take place at [CAV 2020](http://i-cav.org/2020/) in Los Angeles, on July 19th 2020. 


### Organizers

* [Mike Dodds](https://galois.com/team/mike-dodds/) (Galois, Inc)
* [Byron Cook](http://www0.cs.ucl.ac.uk/staff/b.cook/) (Amazon Web Services, University College London)

Please direct inquiries to [Mike Dodds](mailto:miked@galois.com). 

### Topic 

Regulatory compliance is a requirement for many types of software systems. For example, cryptographic systems may be subject to FIPS 140-2 certifications, medical data systems must be HIPAA compliant, financial systems are checked against PCI before deployment, and cloud services used by the US government must achieve FedRAMP designation. Even after software is built and certified, changes to the software, no matter how minor, must often be recertified to ensure that they do not break previously-held assumptions.

Unfortunately, current approaches to compliance are slow-moving, human-driven, and very, very expensive. This pace directly clashes with modern software development, which is characterized by rapid change and enormous scale. For many organizations (including ours) compliance imposes unacceptable cost and delay when shipping industry-strength software. In addition, compliance can perversely result in less reliable software, as bug fixes are delayed by certification processes. 

This workshop will explore two hypotheses: formal methods can automate compliance, and compliance can be a killer application for formal methods. We seek formal methods tools, solutions, capabilities, or techniques that can be inserted into certification processes to make them cheaper, faster, and more rigorous. 

Topics of interest: 

* Case studies for certification and compliance 
* Generating auditable proofs
* Detecting and analyzing changes
* Automatically invalidating and regenerating evidence
* Monitoring system boundaries
* Generating reports suitable for human and machine certifiers
