file:: [DICE-Attestation-Architecture-r23-final_1704725025392_0.pdf](../assets/DICE-Attestation-Architecture-r23-final_1704725025392_0.pdf)
file-path:: ../assets/DICE-Attestation-Architecture-r23-final_1704725025392_0.pdf

- Attester environments can vary widely, ranging from those highly resistant to attack to those having little or no resistance.
  ls-type:: annotation
  hl-page:: 12
  hl-color:: blue
  id:: 659c0b19-ac3c-4841-bc2c-91f37127b9b0
- Configuration options, if set poorly, can result in a highly resistant environment being operationally less resistant. 
  ls-type:: annotation
  hl-page:: 12
  hl-color:: blue
  id:: 659c0b20-5400-4491-ba20-4f752f52dace
- A trustworthiness assertion is information that describes the properties of a device that affects the Verifier or Relying Party perception of the device’s integrity. 
  ls-type:: annotation
  hl-page:: 12
  hl-color:: blue
  id:: 659c0b31-8594-40db-b2cc-03ddd3c75640
- Components are often linked and composed to form computational pipelines, arrays, networks, etc. Not every component is expected to be capable of attestation and attestation capable components may not be capable of attesting to every computing element that interacts with the computing environment.
  ls-type:: annotation
  hl-page:: 12
  hl-color:: blue
  id:: 659c0b49-8ea5-4a09-a10b-ff6098225e90
- ATTESTATION ARCHITECTURE
  ls-type:: annotation
  hl-page:: 13
  hl-color:: blue
  id:: 659c0c0a-d6c2-43d5-9cd9-cb229da4d674
- Roles are performed by actors. Actors are deployed entities.
  ls-type:: annotation
  hl-page:: 13
  hl-color:: blue
  id:: 659c0c27-53cf-4221-8a35-819a02348bb6
- Attestation Roles
  ls-type:: annotation
  hl-page:: 14
  hl-color:: blue
  id:: 659c0c5f-1fcd-4ec4-a368-e60ab9fa27b6
- The attestation roles architecture primarily focuses on the trust model elements of a system. There are five roles defined by the attestation roles architecture, as illustrated in Figure 1. Roles consume and/or produce attestation related information. There are a variety of possible configurations in which role interactions may occur.
  ls-type:: annotation
  hl-page:: 14
  hl-color:: blue
  id:: 659ee948-295f-4d6e-aa5f-f625ab12a458
- Role Messages
  ls-type:: annotation
  hl-page:: 16
  hl-color:: blue
  id:: 659eeb38-7bff-460c-989c-91957a4febf3
- 5.3 Topology Models
  ls-type:: annotation
  hl-page:: 18
  hl-color:: blue
  id:: 659eeb9c-ef32-45e2-af79-32a2844e8426
- 5.4 Assignment of Roles to Actors
  ls-type:: annotation
  hl-page:: 20
  hl-color:: blue
  id:: 659eebc5-2905-4d10-93e6-a8478a00448a
- Entities that implement Attestation Roles are known as Actors. There are many possible ways to assign roles to Actors. This section identifies common patterns involving role-actor combinations. Actor entities are the deployment environments that host and implement attestation roles (e.g., users, organizations, execution environments, service providers, servers, networks, devices, TEEs, DICE layers, Roots of Trust, etc.).
  ls-type:: annotation
  hl-page:: 20
  hl-color:: blue
  id:: 659eebda-5d6b-49cb-95cb-7bc699bf94e2
- 5.4.1 Role-Actor Composition
  ls-type:: annotation
  hl-page:: 21
  hl-color:: blue
  id:: 659eed25-82c4-4a85-8c38-08fce81bde26
- 6 Layered Device Attestation
  ls-type:: annotation
  hl-page:: 26
  hl-color:: blue
  id:: 659eed84-4972-4183-a023-775e27b109b1
- Layered attestation refers to the traversal of DICE layers where the current layer attests to the state of the next layer. Evidence about the next layer is signed by the current layer. Trust in a current DICE layer depends on the trustworthiness of all previous layers.
  ls-type:: annotation
  hl-page:: 26
  hl-color:: blue
  id:: 659eeda6-7d76-43db-8a80-e8d44d009432
- 6.1 Evidence as X.509 Certificate Extensions
  ls-type:: annotation
  hl-page:: 26
  hl-color:: blue
  id:: 659eedbf-a189-46c1-bf13-faac7d1079ce
- The declaration of DiceTcbInfo is:
  ls-type:: annotation
  hl-page:: 28
  hl-color:: blue
  id:: 659eedfa-7c2e-4457-a564-f39972da9dd3
- When filling in the DiceTcbInfo extension, the issuer (layer N) must ensure that any non-constant field contributes to the CDI that generated the subject key (such that a change in the value will cause a change in the CDI). For nonconstant fields, the issuer must ensure that it derives the value by measuring the subject layer (layer N+1).
  ls-type:: annotation
  hl-page:: 29
  hl-color:: blue
  id:: 659eeea3-1bc6-46e0-a64f-b95a2aea5024
- 6.1.2 Multiple DiceTcbInfo Structures Extension
  ls-type:: annotation
  hl-page:: 30
  hl-color:: blue
  id:: 659eeec6-0917-4d7c-be42-14db97cd660d
- The initial state of a DICE TCB may be represented by multiple measurements, for example when it is composed of elements supplied by different vendors or when other inputs (for example fuse state) that affect the functionality of the TCB need to be measured. This certificate extension defines a sequence of DiceTcbInfo structures, one for each measurement
  ls-type:: annotation
  hl-page:: 30
  hl-color:: blue
  id:: 659eeed4-341e-40e2-aab5-37ed87f845fe
  hl-stamp:: 1704914647694
- 6.1.3 UEID Evidence Extension
  ls-type:: annotation
  hl-page:: 30
  hl-color:: blue
  id:: 659ef0db-bb0d-484c-9f96-6ec79b5d1fbb
- 6.1.4 CWT Claims Set Evidence Extension
  ls-type:: annotation
  hl-page:: 30
  hl-color:: blue
  id:: 659ef0ee-7925-4e38-ab47-25edd1a46fd8
- The CBOR Web Token (CWT) specification [10] defines a CBOR encoding of a claim set that may be used to contain Evidence. A variant of CWT does not contain integrity protection; Unprotected CWT Claims Set (UCCS) defines a certificate Evidence extension containing UCCS formatted Evidence.
  ls-type:: annotation
  hl-page:: 30
  hl-color:: blue
  id:: 659ef148-825e-4cb5-bec9-8f9b15e3dc62
- 6.1.5 Manifest Evidence Extension
  ls-type:: annotation
  hl-page:: 31
  hl-color:: blue
  id:: 659ef162-bea5-4a6b-a66b-39bf9ae1dbb7
- A SWID or CoSWID manifest may be used to contain Evidence.
  ls-type:: annotation
  hl-page:: 31
  hl-color:: blue
  id:: 659ef341-6558-488d-a1c8-e2047e4f826a
- Attestation Verifiers require attestation reference values. Endorsers (i.e., manufacturers and suppliers) create Endorsements that can be used as reference values by a Verifier seeking to compare Evidence to values that correspond to a manufacturer’s result. Endorsements may also contain assertions that are not contained in Evidence but may be required by an Appraisal Policy. This specification specifies the following approaches for encoding Endorsements:(i) X.509 identity certificate extensions containing Endorsement values.(ii) X.509 attribute certificates containing Endorsement values.(iii) CoSWID manifest containing Endorsement values.
  ls-type:: annotation
  hl-page:: 31
  hl-color:: blue
  id:: 659ef3b3-9885-47b3-9806-c29da05dbf1b
- 6.5.1.1 Manifest as an X.509 Certificate Extension X.509 certificates [7] allow extensions that may contain additional information. Endorsement values may be conveyed using certificate extensions. This extension contains a manifest structure that is signed by an Endorser. The manifest contains reference values about the target TCB. The manifest can be used by a Verifier to appraise Evidence contained in a DiceTcbInfo extension. The declaration of DiceEndorsementManifest is as follows: The Manifest Format fields are:• format – defines the manifest schema and encoding format: o swid-xml – manifest contains an XML [11] encoded SWID Tag manifest as defined by [12]. o coswid-cbor – manifest contains a CBOR [8] encoded CoSWID manifest as defined by [9]. o coswid-json – manifest contains a JSON [13] encoded CoSWID manifest.• manifest – a signed or not signed manifest containing endorsement or evidence claims about a TCB.
  ls-type:: annotation
  hl-page:: 32
  hl-color:: blue
  id:: 659ef3d2-4556-46d8-be84-fb86b7bcf50e
- 7 Attesting Environment
  ls-type:: annotation
  hl-page:: 34
  hl-color:: blue
  id:: 659ef3e8-d86b-4c03-8c9a-1596cd4ce95a
- 7.1 Compound Device Identifiers
  ls-type:: annotation
  hl-page:: 34
  hl-color:: blue
  id:: 659ef402-bcc9-45aa-88f4-a887e1b1a380
- The Attesting Environment (i.e., the issuer of Evidence) MUST ensure that each non-constant evidence field has contributed to a corresponding CDI value. If a CDI value of an Attester changes, then at least one non-constant evidence field has also changed, and vice versa. This ensures consistency between what is asserted as Evidence and actual conditions described by Evidence
  ls-type:: annotation
  hl-page:: 34
  hl-color:: blue
  id:: 659ef416-06af-4e05-bec0-a899031ce9b2
- 7.2 Security Validation
  ls-type:: annotation
  hl-page:: 34
  hl-color:: blue
  id:: 659ef42f-c749-4701-9f18-bbf3419da0d2
- It is often necessary or desirable to ensure an Attester, and therefore, an Attesting Environment, has been validated and complies with a standard set of security requirements. The Federal Information Processing Standard (FIPS) Publication 140-3 [16] is one important example. It is a U.S. government standard that defines minimum security requirements for cryptographic modules in information technology products. This section provides guidance to help facilitate compliance for DICE-based Attesters.
  ls-type:: annotation
  hl-page:: 34
  hl-color:: blue
  id:: 659ef44a-4cb9-486e-a259-d63e7ce0b239
- For DICE implementations in which in which it is not possible or desirable to reinstantiate the DRBG with the same random seed on each power-on reset cycle, an asymmetric key of any DICE type (ECA, attestation, identity) can be generated exactly once and stored. The dependency of the generated keys on a CDI is achieved by inputting its creation components into the DRBG as shown in Figure 13. After generated keys are created, they can be stored instead of being regenerated by reusing DRBG state. A retrieval mechanism can be used to protect the generated keys.
  ls-type:: annotation
  hl-page:: 34
  hl-color:: blue
  id:: 659ef47e-6000-438e-b283-7d2084e601da
- A key retrieval mechanism controls access to stored asymmetric keys. One way to control access is to encrypt an asymmetric key with an encryption key linked to the creation components of the asymmetric key.
  ls-type:: annotation
  hl-page:: 35
  hl-color:: blue
  id:: 659ef4a5-378e-48cf-8590-3b23b3602d9d
- The strength of this retrieval mechanism is dependent on the combination of selected encryption, key derivation, and integrity protection algorithms.
  ls-type:: annotation
  hl-page:: 35
  hl-color:: blue
  id:: 659ef4c4-4853-42a8-94a0-48971cd48db9
- 7.3 Evidence
  ls-type:: annotation
  hl-page:: 36
  hl-color:: blue
  id:: 659ef4dc-cb27-4761-94ba-d55c3107562e