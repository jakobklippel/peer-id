# peer-id
A decentralized identity verification protocol

PeerID is a decentralized, anonymous identity verification protocol that aims to prevent online misinformation, manipulation, and fraud. By using Peer-ID, users can assure others that the content they interact with is real and trustworthy, without sacrificing privacy and anonymity.

## Whitepaper


### I. Introduction

### Background and Context

Identity verification solutions are crucial in the digital age as they enable the identification of misinformation, computer-generated content, and help build trust in online interactions. However, common identity verification systems have several shortcomings, including being non-anonymous. Some more anonymous systems have shortcomings regarding privacy, security and accessibility. Additionally, with the rise of AI and machine learning technologies, it has become easier for malicious actors to create convincing fake identities and manipulate content online, making it even more difficult to ensure the authenticity of online identities.

To address these challenges, innovative and secure approaches to online identity verification are needed. Other decentralized identity solutions have compromised on usability, accessibility, privacy, and cost, making them less effective and less widely adopted. The PeerID protocol aims to address these shortcomings by providing a decentralized, anonymous, and secure identity verification system that prioritizes practicability and resistance to manipulation and censorship.

### Problem Statement and Motivation

The prevalence of misinformation, manipulation, and fraud online undermines trust and damages the integrity of online communities. Traditional centralized identity verification systems require users to provide personal information, compromising their privacy and leaving them vulnerable to data breaches. Additionally, these systems can be manipulated by bad actors, who can create fake identities and spread false information online. With the increasing sophistication of AI technology, online verification methods are becoming less reliable, creating a need for more innovative and secure approaches to identity verification. A peer-to-peer, offline verification system is key to a reliable way to prevent manipulation and ensure the authenticity of user identities.

### Objectives and Goals

The PeerID protocol aims to provide a decentralized, anonymous, and secure identity verification system that can prevent online misinformation, manipulation, and fraud. The protocol achieves this objective by allowing users to create and verify their digital identities in a secure and tamper-proof way through a peer-to-peer verification process. This involves a physical, in person meeting where both parties confirm the identity shown by the other through a signing process. The verified identities are stored in a decentralized manner on a distributed ledger, ensuring the authenticity and integrity of the data. 

PeerID aims to enhance trust and transparency in online communities, enabling users to make more informed decisions and build stronger relationships. The project is open source and community-driven, with the goal of creating a protocol that is accessible and useful to all.

### II. Technical Overview

The PeerID protocol enables users to create and verify their digital identities in a secure and tamper-proof way through a peer-to-peer verification process. This involves users showing a picture of themselves to the other user through a P2P connection. No personal data, official ID, or other sensitive information is required to be shared with the verifying peer. The picture is only sent to the device of the verification partner and is not stored anywhere else. The verified identities are then stored on a distributed ledger, which is maintained by a network of nodes that validate transactions and ensure the consistency and security of the data.

#### Components

The PeerID protocol has several key components that work together to provide a secure and decentralized identity verification system. These components include a mobile client application, distributed ledger technology (DLT), an oracle analysis service, a decentralized anonymiser application (DApp), and a public identity provider .

##### Client Applications

Client applications are mobile applications that users install on their devices to create and verify their digital identities. The client applications provide a user-friendly interface for users to interact with the protocol, including the ability to initiate and complete the peer-to-peer verification process.

##### Distributed Ledger Technology (DLT)

Verification data is stored on a DLT, which provides a secure and tamper-proof way to store and share information. The use of DLT ensures that the verified identities are decentralized, and no central authority controls or owns the data.

##### Oracle Service

The PeerID protocol uses an oracle service to analyze the verification data stored on the DLT and calculates individual trust scores for each user. The trust score is a measure of the user's reputation and credibility within the network, based on the number of verifications they have completed and the ratings they have received from other users.

Since it is expected that analysis methods and weights might need to adapt to external changes, this service will be centralised, but controlled though a decentralized, autonomous organisation (DAO). The protocol allows for multiple, alternative and independent oracle services to be utilised, making the system less dependent on a single entity.  

##### Decentralized Application (DApp)

The DApp anonymizes user identities and trust scores using zero-knowledge proofs, ensuring user privacy and anonymity. Users can prove that they are unique, human, and have a certain trust score without revealing any personal information. The use of zero-knowledge proofs ensures that the identity of users cannot be traced back to the verifying peers, and the users' behavior cannot be tracked cross services.

##### Identity provider

The PeerID protocol provides an identity provider that can be integrated with third-party services. This allows users to use their verified identities to access other services without having to create new accounts or undergo additional verification processes.

Identities can also be used to add signatures to online content such as image, video, audio, or text. By doing so they claim ownership of given content and signal trustworthiness to others without sacrificing anonymity. 

#### Design decisions and trade-offs

The design decisions of PeerID were made with a focus on accessibility, reliability, privacy, and resistance to manipulation and censorship. To achieve this, biometric data will not be used due to cost, privacy concerns, and accessibility. Instead, the PeerID protocol requires users to engage in peer-to-peer verifications with people they choose and trust. While this may reduce the ability to automatically identify duplicate profiles and reliability of individual verifications, it allows more users to participate in the service. Given there are multiple, confirming verification from different peers, a very high verification confidence can be reached that even exceeds biometric methods. Additionally, the protocol does not rely on centralized ID verification services, which are expensive and can compromise privacy. Instead, individual verifications are done peer-to-peer and stored on a DLT. To strengthen the whole system, some selected users that agree to do so will participate in centralized ID verifications during the initial phase where the network has less coverage and lacks local verification interactions. Lastly, there is no online verification process, as online information can be easily manipulated or faked, especially with modern AI technology. While this makes the verification process less accessible and more complex, it ensures that the identity verification is reliable and resistant to manipulation from the start on.

While there will always be trade-offs, PeerId aims to provide the optimal balance in terms of practicability while maintaining high, temper-proof security. 
