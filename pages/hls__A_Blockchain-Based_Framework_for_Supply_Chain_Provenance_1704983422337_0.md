file:: [A_Blockchain-Based_Framework_for_Supply_Chain_Provenance_1704983422337_0.pdf](../assets/A_Blockchain-Based_Framework_for_Supply_Chain_Provenance_1704983422337_0.pdf)
file-path:: ../assets/A_Blockchain-Based_Framework_for_Supply_Chain_Provenance_1704983422337_0.pdf

- Information Handling Services reported that the potential annual risk of the global supply chain from counterfeiting is at$169 billion and increasing
  ls-type:: annotation
  hl-page:: 1
  hl-color:: blue
  id:: 659fff23-f0f5-4e7d-9195-74c581899196
- The detection of a compromised device is extremely challenging as there are a wide variety of parts with different resources already in the supply chain. Finding a one-size-ﬁts-all solution is our primary objective such that the majority of devices can be authenticated using this single solution. Ensuring the security of the supply chain requires the authenticity for all parts, which can be guaranteed if we can track the parts through trusted suppliers back to their true origin.
  ls-type:: annotation
  hl-page:: 2
  hl-color:: blue
  id:: 659fffb8-81ce-49f3-9817-78598f9436ee
- We proposed a novel architecture, which uses a low-cost blockchain instance for providing traceability of electronic parts or devices.
  ls-type:: annotation
  hl-page:: 2
  hl-color:: blue
  id:: 659fffd3-390e-4c54-8d54-42849783b2b6
- Therefore, directly transferring the ownership within one transaction creates irreversible results in the traditional blockchain-based systems, which could cause further security and management risks. To address these aforementioned threats, we propose a conﬁrmation-based ownership transfer in our blockchain-based framework for enabling device traceability. In this proposed framework, a two-transaction-based ownership management is proposed
  ls-type:: annotation
  hl-page:: 2
  hl-color:: blue
  id:: 65a0002e-b682-466e-b841-1bf2deffacac
- A signiﬁcant amount of research has been directed to ensure the security and integrity of the supply chain by the efﬁcient detection and avoidance of counterfeit ICs [1], [18]–[24],[24]–[29]. The approaches can be categorized into different categories – (i) standards [18], [30]–[32], (ii) statistical data analysis [22]–[25], [33], [34], (iii) on-chip sensors and structures [26]–[28], [35]–[38] and (iv) unique markers [39]. Even though these solutions can provide some levels of detection of counterfeit ICs, none of them can provide the traceability information, such as the origin, manufacturer, bill of materials, and travel trace in the supply chain.
  ls-type:: annotation
  hl-page:: 2
  hl-color:: blue
  id:: 65a00056-2780-4d89-a108-5a48942b05c9
- The authors in [52] introduced a blockchain-based framework, which ensures the authenticity of electronics with the help of an unclonable ID generated from a SRAM-based PUF. Xu et al. provided a comprehensive solution and summary for using blockchain to improve and secure the integrity of electronic supply chain [53]. However, these two solutions do not provide detailed traceability and ownership information for a device.
  ls-type:: annotation
  hl-page:: 3
  hl-color:: blue
  id:: 65a000bc-d076-41e0-8da8-6c4567503380
- owever, the device ownership transfer is simply triggered and controlled by device owners. This design may lead to potential security issues. Human errors, delivery and management failures, in-transit thefts, and dishonest participants are still threatening supply chain even with implementation of blockchain for tracking [55].
  ls-type:: annotation
  hl-page:: 3
  hl-color:: blue
  id:: 65a00122-13b9-4846-9d98-c656756594e3
- Figure 1 describes a simpliﬁed version of the supply chain, which consists of ﬁve different types of entities – design authority, contract manufacturer, distributor, end user/customer, and adversary. 
  ls-type:: annotation
  hl-page:: 3
  hl-color:: blue
  id:: 65a00141-7b67-4f85-ae9c-b7a0ac4611dc
- FIGURE 1.
  ls-type:: annotation
  hl-page:: 3
  hl-color:: blue
  id:: 65a00165-8798-481d-96ed-b4ae809a63b4
- FIGURE 2. Proposed blockchain for supply chain provenance
  ls-type:: annotation
  hl-page:: 4
  hl-color:: blue
  id:: 65a0018c-e4d8-4556-b4f7-632b5c30f112
- In this blockchain based system, design authority, contract manufacturers, and distributors are the major members of blockchain and they have to be registered as ‘‘nodes’’ in blockchain.
  ls-type:: annotation
  hl-page:: 4
  hl-color:: blue
  id:: 65a001f0-3273-4c09-a359-4bcdef0cfbb6
- Any other participants like distributors and customers could not register the device type in the system due to the deﬁned blockchain policy.
  ls-type:: annotation
  hl-page:: 5
  hl-color:: blue
  id:: 65a0022f-7573-4a6e-8da2-71d0d513f0ca
- Generally, design authority, contract manufacturers, and distributors are allowed to initiate transactions for the device transfer, as long as they own a certain amount of devices.
  ls-type:: annotation
  hl-page:: 6
  hl-color:: blue
  id:: 65a00297-9d2d-4a0c-b902-b7be4cf3a740
- However, the actual ownership of the device that is declared to be transferred in the device transfer transaction would not be transferred to the new owner until a conﬁrmation transaction is received
  ls-type:: annotation
  hl-page:: 6
  hl-color:: blue
  id:: 65a0030c-e8a9-4a19-96b6-c5e1ddb4d64d
- Whenever a participant physically receives a device, it is required to verify its identity (ID) which is present (hashed) in the blockchain. The veriﬁcation procedure requires the retrieval of the unique device ID, which can be accessed by using JTAG interface [61] or other unique identiﬁcation methods that are tamper proof.
  ls-type:: annotation
  hl-page:: 6
  hl-color:: blue
  id:: 65a0034f-19ad-4678-978b-488d485ee55e