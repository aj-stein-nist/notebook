file:: [NIST.AMS.300-6_1704902270580_0.pdf](../assets/NIST.AMS.300-6_1704902270580_0.pdf)
file-path:: ../assets/NIST.AMS.300-6_1704902270580_0.pdf

- Reference information model for a blockchain-based product data traceability
  ls-type:: annotation
  hl-page:: 9
  hl-color:: blue
  id:: 659ee76f-143e-4642-af70-36e0e4544751
- One way to mitigate those risks is to record Data and Provenance information for every single data exchange Transaction to: i) ensure the data has not been tampered with, ii) identify if/when the data was tampered with, and iii) track back who tampered with the data.
  ls-type:: annotation
  hl-page:: 9
  hl-color:: blue
  id:: 659ee780-3a90-479a-acd2-4cd597cf6ca7
- Fig. 5. Reference information model overview
  ls-type:: annotation
  hl-page:: 9
  hl-color:: blue
  id:: 659ee7a6-bafb-4638-b20b-f96ea674b915
- The Provenance package contains information elements that describe the origin and actors involved in the product data transaction:• A product data transaction is issued by a Resource, with a unique identifier(orgOrPersId), which can be either an Organization or a person in that organization (PersonInOrganization).• A PersonInOrganization has an optional first (firstName), last name(lastName) and email but is required to belong to an organization(belongsTo).• An Organization has an optional name and website url, and a mandatory physical location.• A physical location (Address) is composed of a street, a street number(streetNumber), a town, a region, a postal/zip code (postalCode), a postal box number (postalBox) and a country.
  ls-type:: annotation
  hl-page:: 10
  hl-color:: blue
  id:: 659ee7bc-8ded-476f-8913-20bd6a223fb0
- 3.4. Business rules
  ls-type:: annotation
  hl-page:: 10
  hl-color:: blue
  id:: 659ee7d7-5ef8-466b-abe9-a257c3821544
- The previous sections presented the information artifacts that can be instantiated to represent and describe product data transactions. This section defines a set of business7 This publication is available free of charge from: https://doi.org/10.6028/NIST.AMS.300-6 rules that must be applied to validate instances before they are recorded, in order to maintain a consistent and meaningful repository.
  ls-type:: annotation
  hl-page:: 10
  hl-color:: blue
  id:: 659ee7eb-44aa-4f9b-9e06-915fb118c984
- (2) A person or organization can still send data it does not own, if it was explicitly given that right during the initial acquisition of the data. A SendProductData(SPD1) transaction can be valid if there is a prior SendProductData(SPD2)
  ls-type:: annotation
  hl-page:: 11
  hl-color:: blue
  id:: 659ee7fc-39f0-43f1-8769-bc9da0b8c804
- (3) A person or organization can only claim ownership of a data if no other organization or person has previously claimed ownership of the same data. A RecordOwnership(RO1) transaction is only valid if there is no prior RecordOwnership (RO2) transaction
  ls-type:: annotation
  hl-page:: 11
  hl-color:: blue
  id:: 659ee813-defd-43e4-8520-c1560d9e870d
- Appendix A: Information Model UML Class diagram
  ls-type:: annotation
  hl-page:: 14
  hl-color:: blue
  id:: 659ee833-6529-4122-be44-d615abc7be0e
- Appendix B: Business rules UML Object diagram instantiations
  ls-type:: annotation
  hl-page:: 15
  hl-color:: blue
  id:: 659ee845-3ecc-49b0-9d74-3059cc51d7b9
- Appendix C: BPM Business process
  ls-type:: annotation
  hl-page:: 18
  hl-color:: blue
  id:: 659ee891-1351-469e-a73a-8dc053c38395