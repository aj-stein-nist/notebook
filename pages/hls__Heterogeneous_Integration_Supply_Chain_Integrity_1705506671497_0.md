file:: [Heterogeneous_Integration_Supply_Chain_Integrity_1705506671497_0.pdf](../assets/Heterogeneous_Integration_Supply_Chain_Integrity_1705506671497_0.pdf)
file-path:: ../assets/Heterogeneous_Integration_Supply_Chain_Integrity_1705506671497_0.pdf

- the chiplet and SiP space has grown to meet this demand, creating a new packaging paradigm, advanced packaging, and a new supply chain.
  ls-type:: annotation
  hl-page:: 1
  hl-color:: blue
  id:: 65a7f788-b996-43d7-8436-ec1b3c104b2e
- Our framework utilizes the Chiplet Hardware Security Module to authenticate a SiP throughout its life.
  ls-type:: annotation
  hl-page:: 1
  hl-color:: blue
  id:: 65a7f7b3-b7e0-4305-8827-d9a6f6985aa3
- A GDSII file, a binary file that is useful in representing layout or shapes in hierarchical form, is produced and sent to a foundry to fabricate the SoCs.
  ls-type:: annotation
  hl-page:: 2
  hl-color:: blue
  id:: 65a7f89a-67ba-4169-b1b7-cc3590d9dfe1
- In 2011, it was stated by the U.S. Committee on Armed Services that an estimated 15% of the spare and replacement electronics parts purchased by the Pentagon were counterfeits [32].
  ls-type:: annotation
  hl-page:: 2
  hl-color:: blue
  id:: 65a7f8b3-0a55-4057-af48-a36dd9dc9272
- Since then, the semiconductor industry has only expanded, and new proposed solutions to many of these threats have been developed
  ls-type:: annotation
  hl-page:: 2
  hl-color:: blue
  id:: 65a7f8cf-988d-49bc-a342-6b8abf06fbc1
- Heterogeneous Integration (HI) was proposed to produce ICs with greater functionality per area and performance by incorporating different dies, known as chiplets, which can contain different functionalities and materials, and process nodes onto another die, known as an interposer in either a 2.5D or 3D packaging scheme [15]. Between the interposer and chiplets are redistribution layers, which contain the interconnections between chiplets. This is defined as2.5D packaging, where the chiplets are all located on the same surface.
  ls-type:: annotation
  hl-page:: 2
  hl-color:: blue
  id:: 65a7f986-f989-4538-9385-7b3884de042b
- As heterogeneously integrated chips, named System-in-Packages (SiPs), are gaining attention, there currently lacks an effort to address security concerns with SiPs, as their supply chain is different.
  ls-type:: annotation
  hl-page:: 3
  hl-color:: blue
  id:: 65a7f998-fc55-4350-850f-2c065bd849ab
- The Chiplet Hardware Security Module (CHSM) contains various security primitives and interfacing capabilities all based on prior knowledge of threats in the SoC domain
  ls-type:: annotation
  hl-page:: 3
  hl-color:: blue
  id:: 65a7f9ca-9bd4-408a-891d-51d1354d8244
- Our proposed framework utilizes these two core elements (consortium blockchain and CHSM) to instill integrity in the budding HI supply chain.
  ls-type:: annotation
  hl-page:: 4
  hl-color:: blue
  id:: 65a7f9f6-fb40-4c7f-b065-e27bdb7d25ab
- We leverage existing SoC hardware assets including Electronic Chip Identification(ECID) and Combatting Die and IC Recycling (CDIR) sensors. We also utilize the CHSM within a SiP in the framework for communication with the blockchain and verification of the SiP.
  ls-type:: annotation
  hl-page:: 4
  hl-color:: blue
  id:: 65a7fa23-8b4e-489c-a17d-aa515b7c66f1
- 2.1 SiP Supply Chain
  ls-type:: annotation
  hl-page:: 4
  hl-color:: blue
  id:: 65a7fa45-e6ae-4e90-bd93-6d67057b8849
- 2 BACKGROUND AND PRELIMINARIES
  ls-type:: annotation
  hl-page:: 4
  hl-color:: blue
  id:: 65a7fa50-b040-4398-af77-fb1b873d4074
- The SiP assembly may also choose to test chiplets incrementally as they are integrated to balance yield, the ratio of nondefective/failed instances over the total possible instances, and time of the testing process.
  ls-type:: annotation
  hl-page:: 5
  hl-color:: blue
  id:: 65a7fb74-d47b-4005-b393-a916592281a0
- At the current moment, as the HI supply chain is in its infancy, a variety of companies like Intel, AMD, IBM, TSMC, and Amkor, among others, are involving themselves with different segments of this supply chain.
  ls-type:: annotation
  hl-page:: 5
  hl-color:: blue
  id:: 65a7fb89-7597-4457-ba9e-c3ca97025919
- 2.2 SiP Counterfeit Threats
  ls-type:: annotation
  hl-page:: 5
  hl-color:: blue
  id:: 65a7fbb4-283c-421b-9c1c-126fcf882486
- 2.3 Threat Model
  ls-type:: annotation
  hl-page:: 7
  hl-color:: blue
  id:: 65a7fe53-4db4-479d-aaf4-87e02f7bb7f1
- 2.4 Blockchain
  ls-type:: annotation
  hl-page:: 8
  hl-color:: blue
  id:: 65a7febb-98c6-45e0-aad3-802a57382d56
- Blockchains are nontamperable by lone nodes in the network, which is desirable for IC assurance, as some entities are untrusted and should be incapable of altering significant IC information.
  ls-type:: annotation
  hl-page:: 10
  hl-color:: blue
  id:: 65a7feda-93d0-49c8-a7d1-3a844aafa935
- Most blockchain networks for SoC assurance allow supply chain actors to engage in a consortium to enlist or verify information concerning the SoC throughout the supply chain. Depending on the blockchain, different entities are assumed untrusted and have limited permissions. Trusted entities generally have higher permissions to enroll SoC information with the goal of cross referencing that information later to identify counterfeit SoCs.
  ls-type:: annotation
  hl-page:: 10
  hl-color:: blue
  id:: 65a7fefd-582b-4762-b794-21300b0c08b3
- In this work, SoC information is enrolled by the trusted SoC IP owner/OCM. This includes the public information of the chip, ECID, package markings, and PUF Challenge-Response Pairs (CRPs).
  ls-type:: annotation
  hl-page:: 11
  hl-color:: blue
  id:: 65a7ff15-8353-44de-9ba3-a795fe2f3765
- In another fundamental work, Islam et al. [20] proposed a blockchain framework hosted on Ethereum blockchain utilizing PUF as the means of tracking ICs for assurance.
  ls-type:: annotation
  hl-page:: 11
  hl-color:: blue
  id:: 65a80027-029b-4bbb-8d7d-3056566a2454
- More recently, eChain was proposed to provide a lightweight, hardware requirement-free implementation using Hyperledger Fabric with the same goal in mind [42], providing coverage against recycled, remarked, overproduced, and cloned SoCs.
  ls-type:: annotation
  hl-page:: 11
  hl-color:: blue
  id:: 65a80044-a122-44cf-b54d-81943c504eab
- Extending on eChain, the work of Zhang et al. [50] seeks to identify and mitigate recycled, remarked, tampered bitstream, overproduced, and cloned FPGAs with blockchain.
  ls-type:: annotation
  hl-page:: 11
  hl-color:: blue
  id:: 65a80053-ed65-46f6-ac78-d3b99c32d94a
- 2.5 Chiplet Hardware Security Module
  ls-type:: annotation
  hl-page:: 11
  hl-color:: blue
  id:: 65a80065-567c-4e5e-92b8-1edee47b2889
- Therefore, a root-of-trust chiplet CHSM is required to protect the security assets (cryptographic keys, logic locking keys, unique device ID, protected state control bits, etc.) of the SiP and to prevent information leakage and unauthorized access to the SiP, such as against fault injection attacks.
  ls-type:: annotation
  hl-page:: 11
  hl-color:: blue
  id:: 65a8007a-eb34-44d2-a929-f135ce67a8d6
- During the design phase, the SiP designer designs the CHSM considering the security requirement and design specification of the SiP system, or the SiP designer/trusted assembly procures an existing CHSM from a trusted vendor that satisfies the security requirements. The CHSM chiplet can be implemented in an FPGA platform to be incorporated into a SiP system.
  ls-type:: annotation
  hl-page:: 12
  hl-color:: blue
  id:: 65a801ca-1d34-4d72-8fd2-8fb7083dd085
- We assume that the CHSM is fabricated in an untrusted facility following the horizontal model of the supply chain. However, the trusted assembly house provisions the security assets and the bitstream into the CHSM chiplet.
  ls-type:: annotation
  hl-page:: 12
  hl-color:: blue
  id:: 65a801e1-4e8d-410c-acea-0e7317fee9d9
- The CHSM obtains the data securely from the chiplets and transfers them to the nodes using PKI. However, the interconnections among the CHSM and the chiplets are made through the interposer layer, which is vulnerable to probing attacks (Figure 7) and gets exposed to the attacker if not encrypted. To solve this problem, the CHSM must authenticate the chiplets containing the security assets and communicate in a secure fashion.
  ls-type:: annotation
  hl-page:: 12
  hl-color:: blue
  id:: 65a80212-f39e-4ce1-a875-d5fd26809690
- 2.6 Assumptions
  ls-type:: annotation
  hl-page:: 13
  hl-color:: blue
  id:: 65a80264-9862-4240-bd23-769d8e3bb808
- 3 PROPOSED FRAMEWORK
  ls-type:: annotation
  hl-page:: 13
  hl-color:: blue
  id:: 65a803c0-2112-45fd-b082-ad1b5a3c6945
- With the current lack of availability of SiPs or SiP benchmarks to utilize for testing and lack of a produced CHSM, this framework provides a foundation for HI blockchain implementations. As can be seen in Figure 8, our framework contains many of the same blockchain elements of our team’s eChain [42] implementation for providing provenance to SoCs, PCBs, and systems.
  ls-type:: annotation
  hl-page:: 14
  hl-color:: blue
  id:: 65a803f5-f4af-4ce6-9dbe-97cea40aff4a
- 3.1 Architecture
  ls-type:: annotation
  hl-page:: 14
  hl-color:: blue
  id:: 65a80400-9783-4b16-8890-71f010d86b2a
- Many modern chips are already equipped with PKI infrastructures, enabling them to communicate with the internet.
  ls-type:: annotation
  hl-page:: 15
  hl-color:: blue
  id:: 65a80410-4cb0-4121-b8c1-c96e4deb773b
- the CHSM only encrypts critical security information during communication rather than encrypting all internal communications between the CHSM and chiplets that do not involve security assets.
  ls-type:: annotation
  hl-page:: 15
  hl-color:: blue
  id:: 65a804d5-7091-494c-b612-1c159fbe2896
- Table 2. Example World State Including Four Different SiPs Where SiP 1 and SiP 2 Have Three Chiplets Other Than CHSM, and SiP 3 and SiP 4 Have Two Chiplets Other Than CHSM
  ls-type:: annotation
  hl-page:: 16
  hl-color:: blue
  id:: 65a804f1-5ae8-4319-813d-f42c42b067e3
- 3.2 Entity Roles and Permissions
  ls-type:: annotation
  hl-page:: 17
  hl-color:: blue
  id:: 65a80559-b7b8-46c0-98e2-d4c7248129be
- 3.3 Processes
  ls-type:: annotation
  hl-page:: 18
  hl-color:: blue
  id:: 65a8057c-ecb1-4459-8041-7c633893eaac
- It is significant to note that the CHSM does not need to be active throughout this process communicating with the blockchain, as the SiP assembly reads the CHSM’s ECID and registers the device through their application.
  ls-type:: annotation
  hl-page:: 18
  hl-color:: blue
  id:: 65a8058f-d2d4-4693-b858-3d932d69b600
- 4 SECURITY ANALYSIS
  ls-type:: annotation
  hl-page:: 19
  hl-color:: blue
  id:: 65a80690-830a-459f-aa66-f08a3f4d8746
- the CHSM sends its current CDIR sensor count that is used alongside the registered CDIR sensor count at the time of SiP assembly to produce a CDIR confidence level as seen in the case study of Vosatka et al. [45] showcasing the confidence modeling approach with CDIR sensor information to identify recycled SiPs.
  ls-type:: annotation
  hl-page:: 19
  hl-color:: blue
  id:: 65a806a5-b84c-4f6c-a5ff-4677fdd4dadc
- The CHSM’s ECID can be used in addition to the enrolled grade code and part number of the product to properly identify a SiP that has been remarked. 
  ls-type:: annotation
  hl-page:: 21
  hl-color:: blue
  id:: 65a806bb-6d2d-4918-bf1f-4156c541ab37