.. include:: ../common/common_definitions.rst

.. _defined-terms.rst:


Normative Language and Conventions
++++++++++++++++++++++++++++++++++

The key words "MUST", "MUST NOT", "REQUIRED", "SHALL", "SHALL NOT", "SHOULD", "SHOULD NOT", "RECOMMENDED", "NOT RECOMMENDED", "MAY", and "OPTIONAL" in this document are to be interpreted as described in BCP 14 [RFC2119] [RFC8174] when, and only when, they appear in all capitals, as shown here.


Defined Terms
+++++++++++++

The terms *User*, *Trust Service*, *Trust Model*, *Trusted List*, *Trust Framework*, *Attribute*, *Electronic Attestations of Attributes Provider* or *Trust Service Provider (TSP)*, *Person Identification Data (PID)*, *Revocation List*, *Qualified Electronic Attestations of Attributes Provider* or *Qualified Trust Service Provider (QTSP)*, *Electronic Attestation of Attributes (EAA)*, are defined in the `EIDAS-ARF`_.

Below are the description of acronyms and definitions which are useful for further insights into topics that complement the it-wallet and the interacting components.

.. list-table::
   :header-rows: 1

   * - Name
     - Description
     - Notes
   * - User
     - A natural or legal person, or a natural person representing another natural person or a legal person, that uses a trust services or electronic identification means provided in accordance with EUDI Wallet Architecture Reference Framework. 
     - | Aligned with ARF v1.4. 
       |
       | *Alternative terms:* EUDI Wallet User.
   * - User Attribute
     - A characteristic, quality, right or permission of a natural or legal person or of an object. 
     - | Aligned with ARF v1.4.
       | 
       | *Alternative terms:* Attribute, User Claim.
   * - Digital Identity Provider
     - Entity responsible for identifying citizens for the issuance of a digital identity.
     - 
   * - Digital Credential
     - A signed set of Attributes encapsulated in a specific data format, such as mDoc-CBOR format specified in [ISO 18013-5] or the SD-JWT VC format specified in [SD-JWT-VC]. This may be a Personal Identification Data (PID), (Qualified) Electronic Attestation of Attribute ((Q)EAA). 
     - | Revised from ARF v1.4.
       | *Differences:* The definition from ARF restricts the data format to mDoc-CBOR and SD-JWT VC. A Digital Credential definition should be neutral on the format. 
       |
       | *Alternative terms:* Electronic Attestation, Attestation, Verifiable Credential, Digital Attestation.
   * - Organizational Entity
     - A legal person (only considering organizations and public entities, not natural/physical persons) recognized by the Member State through a unique identifier to operate a certain role within the EUDI Wallet ecosystem.
     - | In this category the following entity roles are included: Wallet Provider, Credential Issuer, Relying Party, QTSP In general, any kind of Entity that must be registered through a national or European registration mechanism. 
       |
       | *Alternative terms:* legal person (only considering organizations and public entities, not natural/physical persons).
   * - Wallet Solution
     - A Wallet Solution is the entire eIDAS-compliant product (combination of software, hardware, services and settings) provided by a Wallet Provider to Users and certified as EUDI-compliant by a Conformity Assessment Body (CAB). 
     - | Revised from ARF v1.4 and Implementing Act.
       | *Differences:* editorial. 
       |
       | *Alternative terms:* EUDI Wallet Solution.
   * - Wallet Unit
     - Unique configuration of a Wallet Solution that includes Wallet Instances, WSCAs, and WSCDs provided by a Wallet Provider to an individual Wallet User. For device-based WSCD implementations like TEEs, the Wallet Provider may not supply the WSCD itself.
     - | A Wallet Unit should be understood as a specific setup of the Wallet Solution for an individual User. It should include the application installed on a Wallet User's device or environment that the Wallet User interacts with directly (the Wallet Instance) and the necessary security features to protect the user's data and transactions. These security features should involve special software or hardware to encrypt and safeguard sensitive information.
       |
       | Revised from Implementing Act.
       | *Differences:* added sentence that specify that a Wallet Provider may not supply the WSCD. 
   * - Wallet Provider
     - An Organizational Entity, responsible for the management and provisioning of a Wallet Solution. 
     - | Revised from ARF v1.4 and Implementing Act.
       | *Differences:* editorial (use of Organizational Entity instead of public or private organisation and natural or legal person, respectively). 
       |
       | *Alternative terms:* EUDI Wallet Provider.
   * - Wallet Instance
     - It is an application installed and configured on a User's device belonging to and which is controlled by a User, as part of the Wallet Unit. The Wallet Instance provides graphical interfaces for User interaction with the Wallet Unit.
     - | Revised from Implementing Act.
       | *Differences:* editorial. 
       | 
       | *Alternative terms:* EUDI Wallet Instance.
   * - Wallet Provider Backend
     - Is the technical infrastructure and server-side components, including a set of endpoints, managed by a Wallet Provider.
     -
   * - Credential Issuer
     - An Organizational Entity providing Digital Credentials to Users. It may be PID Provider or (Q)EAA Providers. 
     - | Revised from ARF v1.4.
       | *Differences:* (i) merged the PID Providers and (Q)EEA Providers definitions using the general term Digital Credential, (ii) renamed “Member Stare or other legal entity” in “Organizational Entity” ARF alternative terms: PID Providers,(Q)EEA Providers, Attestation Provider. 
       |
       | *Alternative terms:* Verifiable Credential Issuer.
   * - Relying Party
     - An Organizational Entity that relies upon an electronic identification or a Trust Service originating from a Wallet Instance. 
     - | Revised from ARF v1.4. 
       | *Differences:* renamed “natural or legal person” in “Organizational Entity”.
   * - Relying Party Instance
     - A Relying Party Instance in the context of a mobile application or a standalone embedded device refers to a specific deployment of the application or device. These instances depend on an User Authentication through a Wallet Instance to confirm User identities before granting access to their functionalities. Each version or environment where the application or device is running, be it a particular release of a mobile app installed on a User's smartphone or a specific embedded device in use, constitutes a separate instance. In case of proximity supervised scenarios, it belongs to and is controlled by a Verifier. 
     - | Revised from ARF v1.4.
       | *Differences:* added a sentence on proximity supervised scenarios. 
       |
       | *Alternative terms:* Verifier App.
   * - Verifier
     - Also known as Credential Verifier. It is a natural person or a legal person using an Relying Party Instance. 
     -
   * - Trust
     - Trust, within the technical field, is the confidence in the security, reliability, and integrity of entities (such as systems, organizations, or individuals) and their actions, ensuring that they will operate as expected in a secure and predictable manner. It is often established through empirical proof, such as past performance, security certifications, or transparent operational practices, which demonstrate a track record of adherence to security standards and ethical conduct. 
     - | Revised from ARF v1.4.
       | *Differences:* editorial.
   * - Trust Framework
     - A legally enforceable set of operational and technical rules and agreements that govern a multi-party system designed for conducting specific types of transactions among a community of participants and bound by a common set of requirements. 
     - Aligned with ARF v1.4. 
   * - Trust Model
     - Collection of rules that ensure the legitimacy of the components and the entities involved in the EUDI Wallet ecosystem. 
     - Aligned with ARF v1.4. 
   * - Trusted List
     - Repository of information about authoritative entities in a particular legal or contractual context which provides information about their current and historical status. It serves as the bedrock of trust, acting as federative sources that publish the crucial information about root entities within the ecosystem.    
     - | Revised from ARF v1.4.
       | *Differences:* added the last sentence.
   * - Registration Authority
     - A party responsible for registering all the Organizational Entities by issuing a Trust Assertion.
     - *Alternative terms:* Registrar.
   * - Conformity Assessment Body (CAB)
     - A conformity assessment body as defined in Article 2, point 13, of Regulation (EC) No 765/2008, which is accredited in accordance with that Regulation as competent to carry out conformity assessment of a qualified trust service provider and the qualified trust services it provides, or as competent to carry out certification of European Digital Identity Wallets or electronic identification means. 
     - Aligned with ARF v1.4.
   * - National Accreditation Bodies (NAB)
     - A body that performs accreditation with authority derived from a Member State under Regulation (EC) No 765/2008. 
     - | Aligned with ARF v1.4.
       |
       | *Alternative terms:* Accreditation Authority.
   * - Trust Evaluation
     - The process of verifying the trustworthiness of registered Organizational Entities, in accordance with pre-established rules. For example, involving the retrieval and validation of entity configurations and trust chains.
     - *Alternative terms:* Trust Discovery, Trust Establishment.
   * - Trust Assertion
     - Cryptographically verifiable artifact that proves the compliance of an Organizational Entity with known rules and requirements defined within the Trust Model.
     - *Alternative terms:* Verifiable Attestation, Access Certificate.
   * - Trust Relationship
     - Positive outcome of Trust Evaluation, which produces a reliable relationship between Organizational Entities, where one Organizational Entity trusts the other to securely handle data, execute transactions, or perform actions on its behalf.
     -
   * - Metadata
     - Digital artifact that contains all the required information about an Organizational Entity, e.g., protocol related endpoints and the Organizational Entity’s cryptographic public keys (for the complete list check requirement "Metadata Content").
     -
   * - Policy Language
     - A formal language used to define security, privacy, and identity management policies that govern interactions and transactions within a Trust Framework. This language allows for the clear and unambiguous expression of rules and conditions, facilitating the automation of processes and interoperability among different systems and organizations.
     -
   * - Registration Process
     - Process performed by a Registration Authority verifying necessary information to ensure Organizational Entity eligibility and compliance with the relevant rules and standards. The main goal of the Registration Process is for the Organizational Entity to receive one or more Trust Assertions to be used for the Trust Evaluation processes.
     -
   * - Accreditation Process
     - Process performed by the National Accreditation Body to accreditate CABs. As a result of the Accreditation Process, a NAB issues an accreditation certificate to a CAB.
     - 
   * - Certification Process
     - Process performed by Conformity Assessment Bodies to certify the Wallet Solution. The Certification Process aims to periodically assess technical Wallet Solutions (e.g. performing vulnerability assessment and risk analysis). As a result of the Certification Process a certification is provided to the Wallet Solution. 
     - 
   * - Notification Process
     - Process defining how information is transferred to the European Commission and the inclusion of an entity in the Trusted List.
     -
   * - Supervision Process
     - Process performed by a Supervisory Body to review and ensure proper functioning of the Wallet Provider and other relevant actors.
     - 
   * - Federation Authority
     - A public governance entity that issues guidelines and technical rules, and administers - directly or through its intermediary - Trusted Lists, services, and accreditation processes, the status of participants, and their eligibility evaluation. It also performs oversight functions.
     -
   * - Critical Assets
     - They are assets within or in relation to a Wallet Unit (for example cryptographic keys) of such importance that their incapacitation or destruction would have a very serious, debilitating effect on the ability to rely on the Wallet Unit.
     - | Revised from Implementing Act.
       | *Differences:* editorial. 
   * - Wallet Secure Cryptographic Application (WSCA)
     - An application that manages Critical Assets utilizing the cryptographic functions provided by the WSCD.
     - | The type of WSCAs depends on the type of WSCD. For example, it might be an eUICC or JavaCard applet for a local UICC or an external JavaCard-based smart card solution, while in a local Android hardware-backed Keystore solution, native trusted applications may function as the WSCA.
       |
       | Revised from Implementing Act.
       | *Differences:* editorial. 
   * - Wallet Unit Attestation
     -  It is a data object issued by a Wallet Provider that describes the components of the Wallet Unit. It allows authentication and validation of those components, and is cryptographically bound to Wallet Secure Cryptographic Devices.
     - *Alternative terms:* Wallet Attestation or Wallet Instance Attestation.
   * - Wallet Secure Cryptographic Device (WSCD)
     - It is a tamper-resistant device that provides an environment that is linked to and used by the WSCA to protect Critical Assets and provide cryptographic functions for the secure execution of critical operations. 
     - | Example of WSCD type are: remote solutions (e.g., HSMs), local external solutions (e.g., smart cards), local device-integrated solutions (e.g., UICC or native cryptographic hardware, such as the iOS Secure Enclave, Android Hardware Backed Keystore or StrongBox), and hybrid solutions that combine two or more of these types. 
       |
       | Aligned with Implementing Act.
   * - Credential Status Assertion
     - Signed document serving as proof of a Digital Credential's current validity status.
     -
   * - Device Integrity Service
     - A service provided by device manufacturers that verifies the integrity and authenticity of the app instance (Wallet Instance), as well as certifying the secure storage of private keys generated by the device within its dedicated hardware. It's important to note that the terminology used to describe this service varies among manufacturers.
     -
   * - Cryptographic Hardware Keys
     - During the app initialization, the Wallet Instance generates a pair of keys, one public and one private, which remain valid for the entire duration of the Wallet Instance's life. Functioning as a Master Key for the personal device, these Cryptographic Hardware Keys are confined to the OS domain and are not designed for signing arbitrary payloads. Their primary role is to provide a unique identification for each Wallet Instance.
     -
   * - Cryptographic Hardware Key Tag
     - A unique identifier created by the operating system for the Cryptographic Hardware Keys, utilized to gain access to the private key stored in the hardware.
     -
   * - Key Attestation
     - An attestation from the device's OEM that enhances your confidence in the keys used in your Wallet Instance being securely stored within the device's hardware-backed keystore. Its content is therefore defined by the operating system manufacturer. For Google Android, the term Key Attestation refers to the Strongbox Key Attestation feature. For Apple iOS, the reference is to the `Device Check`_ service, specifically the `attestKey`_ feature.
     -
   * - Qualified Electronic Attestation of Attributes (QEAA)
     - A digitally verifiable attestation in electronic form, issued by a QTSP, that substantiates a person's possession of attributes.
     -
   * - Qualified Electronic Signature Provider
     - The Electronic Trust Service Provider responsible for the issuing of Qualified Electronic Signature certificates to the User.
     -
   * - Qualified Electronic Attestation of Attributes Provider
     - Organizational Entity which serves as Credential issuer providing Qualified Electronic Attestations of Attributes (QEAAs).
     - 
   * - PID Provider
     - A Credential Issuer responsible for issuing and revoking Person Identification Data (PID) to Users, ensuring that the PID of a User is cryptographically bound to a Wallet Unit. 
     - | Revised from ARF v1.4 and Implementing Act.
       | *Differences:* editorial (renamed “Member Stare or other legal entity” and "natural or legal person", respectively).
   * - National Identity Provider
     - It represents preexisting identity systems based on SAML2 or OpenID Connect Core 1.0, already in production in each Member State (eg: the Italian SPID and CIE id schemes notified eIDAS with *LoA* **High**, see `SPID/CIE-OpenID-Connect-Specifications`_).
     -
   * - Trust Attestation
     - Electronic attestation of an entity's compliance with the national regulatory framework, which is cryptographically verifiable and cannot be repudiated over time by the entity that issued it. A Trust Attestation is always related to a particular Trust Framework.
     -
   * - Trust Layer
     - Architectural component that enables IT-Wallet system participants to establish trust, in terms of reliability and compliance of all participants with the regulatory framework governing the digital identity system.
     -
   * - Trust Model
     - System defining how the participants of the ecosystem establish and maintain trust in their interactions. The Trust Model outlines the rules and the procedures for the entities (like users, systems, or applications) should validate each other's identities, authenticate, and establish the level of trust before exchanging information.
     -
   * - Level of Assurance
     - The degree of confidence in the vetting process used to establish the identity of the User and the degree of confidence that the User who presents the credential is the same User to whom the Digital Credential was issued.
     -
   * - Holder Key Binding
     - Ability of the Holder to prove legitimate possession of the private part, related to the public part attested by a Trusted Third Party.
     -
   * - Holder
     - Natural or Legal person that receives Verifiable Credentials from the Credential Issuers, manages the Verifiable Credentials within the Wallet, and presents them to Verifiers. The Holder is the User in control of the Wallet.
     -
   * - Pseudonym
     - Pseudonyms are alternative identifier used to represent an entity (such as a person or organization) without revealing their true identity. It provides a layer of privacy and anonymity while still allowing for consistent authentication and authorization within a system.
     -


Acronyms
--------

.. list-table::
  :widths: 20 80
  :header-rows: 1

  * - **Acronym**
    - **Description**
  * - **OID4VP**
    - OpenID for Verifiable Presentation
  * - **PID**
    - Person Identification Data
  * - **VC**
    - Verifiable Credential
  * - **VP**
    - Verifiable Presentation
  * - **API**
    - Application Programming Interface
  * - **LoA**
    - Level of Assurance
  * - **AAL**
    - Authenticator Assurance Level as defined in `<https://csrc.nist.gov/glossary/term/authenticator_assurance_level>`_
  * - **PII**
    - Personally Identifiable Information
  * - **WSCD**
    - Wallet Secure Cryptographic Device
  * - **WSCA**
    - Wallet Secure Cryptographic Application
  * - **CIE**
    - National Electronic Identity Card
  * - **SPID**
    - Italian Public Digital Identity System
  * - **ANPR**
    - Italian National Registry of the Resident Population

