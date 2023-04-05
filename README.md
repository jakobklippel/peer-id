# PeerID
Peer Identity Verification Protocol

PeerID is a anonymous identity verification protocol that aims to prevent online misinformation, manipulation, and fraud. By using PeerID, users can assure others that the content they interact with is real and trustworthy, without sacrificing privacy and anonymity. PeerID specifically offers a reliable way for proof of uniqueness and proof of humanity for online users.

## Whitepaper

### I. Introduction

### Background and Context

Identity verification solutions are becoming more important in the context of AI advancements as they allow to distinguish human from computer-generated content, and thus, help to build trust in online interactions. With the rise of AI and machine learning technologies, it is becoming significantly easier for malicious actors to create convincing fake identities and manipulate content online.

To address these challenges, anonymous, scalable approaches to online identity verification are needed. Other verification and identity solutions compromise on usability, accessibility, privacy, or cost, making them less effective and less widely adopted. The PeerID protocol aims to address these shortcomings and provide an identity verification and validation system that prioritizes anonymity, practicability and large scale adoption.

### Problem Statement and Motivation

The prevalence of misinformation, manipulation, and fraud online undermines trust and damages the integrity of online communities. Traditional centralized identity verification systems require users to provide personal information, compromising their privacy and leaving them vulnerable to data breaches. Other less intrusive systems can often be easiliy manipulated by bad actors. With the increasing sophistication of AI technology, online verification methods are becoming less reliable, creating a need for more innovative and secure approaches. Peer-to-peer, real world verification is the only reliable, tamper-proof, and scalable identity solution that will persist in the age of AI.

### Objectives and Goals

The PeerID protocol aims to provide an anonymous, and secure identity verification system. PeerID aims to enhance trust and transparency in online communities, enabling users to make more informed decisions and build stronger relationships. The project is open source and community-driven, with the goal of creating a protocol that is accessible and useful to all.

### II. Technical Overview

PeerID protocol requires users to create and verify their digital identities in a secure and tamper-proof way through a peer-to-peer verification process. This involves a physical, in person meeting where two parties confirm the identity (picture) shown by the other through a P2P signing process. No additional personal data, official ID, or other sensitive information is required to be shared with the verifying peer. The verification proofs are stored on a distributed ledger, ensuring the authenticity and integrity of the data. 

#### Components

The PeerID protocol has several key components. These components include a mobile client application, distributed ledger technology (DLT), an oracle analysis service, a decentralized anonymiser application (DApp), and a public identity provider.

##### Client Application

The client is a mobile applications that users install on their devices to create and verify their digital identities. The client application provides a user-friendly interface for users to interact with the protocol, including the ability to initiate and complete the peer-to-peer verification process.

##### Distributed Ledger Technology (DLT)

Verification data is stored on a DLT, which provides a secure way to store and share information. The use of DLT ensures that the verified identities are decentralized, and no central authority controls or owns the data.

##### Oracle Service

The PeerID protocol uses an oracle service to analyze the verification data stored on the DLT and calculates individual trust scores for each user. The trust score is a measure of the user's reputation and credibility within the network, based on the number of verifications they have completed.

Since it is expected that analysis methods and weights might need to adapt to external changes, this service is centralised, but controlled though a decentralized, autonomous organisation (DAO). The protocol allows for multiple, alternative and independent oracle services to be utilised, making the system less dependent on a single entity.  

##### Decentralized Application (DApp)

The DApp anonymizes user identities and trust scores using zero-knowledge proofs, ensuring user privacy and anonymity. Users can prove that they are unique, human, and have a certain trust score without revealing any personal information. The use of zero-knowledge proofs ensures that the identity of users cannot be traced back to the verifying peers, and the users' behavior cannot be tracked cross services.

##### Identity provider

The PeerID system includes an OpenID identity provider that can be easily integrated with third-party services. This allows users to use their verified identities to access other services without having to undergo additional verification processes.

Identities can also be used to add signatures to online content such as image, video, audio, or text. By doing so they claim ownership of given content and signal trustworthiness to others without sacrificing anonymity.

##### Short Signatures

Short Signartures allow signing text and media in way that it is minimal invasive and less distracting from the actual content. This is especially important for areas where the content size is limited. Short signatures are basically a reference to the actual signature which is stored on a separate public service.

#### Design decisions and trade-offs

The design decisions of PeerID were made with a focus on balancing the different requirements for an effective identity validation system. Desing decision include:

- Biometric data will not be used due to cost, privacy concerns, and accessibility. Instead, the PeerID protocol requires users to engage in peer-to-peer verifications with people they choose and trust. While this may reduce the ability to automatically identify duplicate profiles and reliability of individual verifications, it allows more users to participate in the service. Given there are multiple, confirming verification from different peers, a very high verification confidence can be reached that even exceeds biometric methods
- The protocol does not rely on centralized ID verification services, which are expensive and can compromise privacy. Instead, individual verifications are done peer-to-peer and stored on a DLT. To strengthen the whole system, some selected users that agree to do so will participate in centralized ID verifications during the initial phase where the network has less coverage and lacks local verifications
- There is no online verification process forseen, as online information can be easily manipulated or faked, especially with modern AI technology. While this makes the verification process more elaborate, it ensures that the identity verification is reliable and resistant to manipulation. Again, selected individuals might be verified online during the ramp up phase to kick start the network.

While there will always be trade-offs, PeerID aims to provide the optimal balance in terms of practicability while maintaining high, temper-proof security. 
