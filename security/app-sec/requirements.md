# Requirements Phase

Software security requirements fall into 2 categories:

  1. SW Security functions (crytography and user authentication functions)
  1. SW properties and behaviours

*The CIA triad and the AAA model*

Use the core to build a security requirements that include General, Operational and Other security requirements:

![Security Requirements](/docs/assets/images/sw_sec_requirements.png)

General:

**Session management**

>Session management requirements are those that ensure that once a session is established, it remains in a state that it will not compromise the security of the software. software. In other words, the established session is not susceptible to any threats to the security policy as it applies to confidentiality, integrity and availability. Session management requirements assure that sessions are not vulnerable to brute force attacks, predictability or Man-in-the-middle hijacking attempts. 

*Paul, Mano. Official (ISC)2 Guide to the CSSLP CBK ((ISC)2 Press) (p. 121)*

**Exception management**

>Software requirements that explicitly address errors and exceptions need to be defined in the software requirements documentation to avoid disclosure threats. 

*Paul, Mano. Official (ISC)2 Guide to the CSSLP CBK ((ISC)2 Press) (p. 122)*

**Configuration management**

>Software configuration parameters and code which makeup the software needs  protection against hackers.
Identifying and capturing configuration settings is vital to ensure that an appropriate level of protection is considered when the software is designed, developed and more importantly when it is deployed.

*Paul, Mano. Official (ISC)2 Guide to the CSSLP CBK ((ISC)2 Press) (p. 122)*

Operational:

**Deployment Environment**

>While eliciting software requirements it is important to also identify and capture  pertinent requirements about the environment in which the software will be deployed.

*Paul, Mano. Official (ISC)2 Guide to the CSSLP CBK ((ISC)2 Press) (p. 124)*

Consider: *internet facing, DMZ, open ports, production privilege level, sensitive data in transit, authentication requirements, existing OS event logging availability*

**Archiving**

Identify the regulatory and business requirement for business continuity

>During the requirements gathering phase, the location, duration and format  of archiving information must be determined.

*Paul, Mano. Official (ISC)2 Guide to the CSSLP CBK ((ISC)2 Press) (p. 125)*

**Anti-piracy**

Identify requirements for code obfuscation, code signing, anti-tampering, and IP protection mechanisms

>Particularly important for shrink-wrap Commercially-Of-The-Shelf (COTS)  software as opposed to business applications developed in-house, anti-piracy  protection requirements should be identified.

*Paul, Mano. Official (ISC)2 Guide to the CSSLP CBK ((ISC)2 Press) (p. 126)*

Other:

**Sequencing and Timing**

Identify sequencing and timing requirements to protect against race conditions of Time of Check/Time of Use (TOC/TOU) attacks

>Sequencing and timing design flaws in software can lead to what is commonly  known as race conditions or Time of Check/Time of Use (TOC/TOU) attacks.  Race conditions are in fact one of the most common flaws observed in software  design.

*Paul, Mano. Official (ISC)2 Guide to the CSSLP CBK ((ISC)2 Press) (p. 126)*

**International**

>When developing software, international requirements need to be factored in.  International requirements can be of two types – legal and technological.
Legal requirements are those requirements that we need to pay attention to  so that we are not in violation of any regulations.
Technical requirements if  the software needs to support multi-lingual, multi-cultural and multi-regional  needs. Character encoding and display direction.

*Paul, Mano. Official (ISC)2 Guide to the CSSLP CBK ((ISC)2 Press) (p. 127)*

**Procurement**

>The identification and determination of software security requirements is no less  important when a decision is made to procure the software instead of building  it in-house.

*Paul, Mano. Official (ISC)2 Guide to the CSSLP CBK ((ISC)2 Press) (p. 128)*