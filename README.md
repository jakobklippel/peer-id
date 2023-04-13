# PeerID
by Jakob Klippel (jakob@config.one)

*The most significant challenge that must be addressed in the age of AI is developing a reliable online proof of humanity.*

## Peer Identity Verification Protocol

PeerID is an decentralized, peer-to-peer identity verification protocol that enables users to provide a reliable proof of humanity without revealing their identity. In other words, users can assure others that the content they interact with is trustworthy, while still maintaining privacy and anonymity.

PeerID aims to reduces the impact of online misinformation, manipulation, and fraud, resulting from increasingly sophisticated AI technology by helping to identify human users and enhanceing trust and transparency in online interactions.

### I. Introduction

### Background and Context

The prevalence of misinformation, manipulation, and fraud online undermines trust and damages the integrity of online communities today. With the advancement of AI, bad actors gain access to tools that can scale their activities substantially. The risk of this development to human interaction online is difficult to predict, but it is likely to increase significantly, probably to an catastrophic extend for some online services such as social media platforms.

Identity verification solutions are becoming significantly more important in this context as they allow to distinguish human from computer-generated content, and thus, help to build trust in online interactions.

### Problem Statement and Motivation

With the increasing sophistication of AI technology, traditional online verification methods in general are becoming less reliable, creating a need for more innovative and secure approaches. It is becoming significantly easier for malicious actors to create convincing fake identities and generate manipulative content online. Existing solutions compromise on important features. Most are unfit to meet the challenges in the context of AI advancements. They are often expensive to use and require users to provide personal information, compromising their privacy and leaving them vulnerable to data breaches. Other less intrusive systems are much more likely subject to manipulation. A scalable solution should be inclusive and accessible to all users worldwide.

PeerID is a peer-to-peer verification protocol that is a reliable, tamper-proof, and scalable identity solution for the future that will persist in the age of AI while maintaining anonymity and privacy of it's users.

The goal of PeerID is to enhance trust and transparency in online communities, enabling users to make more informed decisions and build stronger relationships. PeerID aims to build a protocol that is accessible and useful to all.

### II. Solution

The PeerID protocol requires users to create and verify their digital identities in a secure and tamper-proof way through a peer-to-peer verification process. This involves a physical, in person meeting where two parties confirm the identity (picture) shown by the other through a P2P signing process. No additional personal data, official ID, or other sensitive information is required to be shared with the verifying peer. The digital verification proofs are stored on a distributed ledger, ensuring the authenticity and integrity of the data.

Based on the interactions data of the verifier network a trust score is calculated for each user. The users identity is further anonymised in the process which prevents tracking cross services and makes it impossible to trace back users public identity to their verifier node and thus, to the peers that they interacted with.

An individuals peer-id can be used for authentication, signatures and captchas at third party services as well as serve as a unique application scoped user ID. Thus, third party services using PeerID integrations can assure that users of their service are unique and human.

Users can anonymously proof their uniqueness and humanity to gain access to services, add digital signatures to online content and thus, build trust and develop stronger relationships online.

### Technical Overview

The PeerID protocol has several key components. These components include a mobile client application (Client), distributed ledger technology (DLT) backend, a network oracle service (Oracle), a public identity provider, and digital signatures.

##### Client Application

The client is a mobile applications that users install on their devices to create and verify their digital identities. The client application provides a user-friendly interface for users to interact with the protocol, including the ability to initiate and complete the peer-to-peer verification process.

##### Distributed Ledger Technology (DLT)

Verification data is stored on a DLT, which provides a secure way to store and share information. The use of DLT ensures that the verified identities are decentralized, and no central authority controls or owns the data.

##### Oracle Service

The PeerID protocol uses an oracle service to analyze the verification data stored on the DLT and calculates individual trust scores for each user. The trust score is a measure of the user's reputation and credibility within the network, based on the number of verifications they have completed.

The oracle service then creates zero-knowledge-proofs and provides them to the users client applications. With those, users can prove that they are unique, human, and have a certain trust score without revealing any personal information. The use of zero-knowledge proofs ensures that the identity of users cannot be traced back to the verifying peers, and the users' behavior cannot be tracked cross services.

##### Identity provider

The PeerID system includes an identity provider that can be easily integrated with third-party services. This allows users to use their verified identities to access other services without having to undergo additional verification processes. Users can create one or multiple application scoped identities with their peer-id. They are required to provide their identity proofs to the service at regular intervals to ensure actuality.

##### Digital Signatures

Identities can also be used to add signatures to online content such as image, video, audio, or text. By doing so they claim ownership of given content and signal trustworthiness to others without sacrificing anonymity.

Short Signartures allow signing text and media in way that it is minimal invasive and less distracting from the actual content. This is especially important for areas where the content size is limited. Short signatures are basically a reference to the actual signature which is stored on a separate public service.

### Design decisions and trade-offs

The design decisions of PeerID were made with a focus on balancing the different requirements for an effective identity validation system. Design decision include:

- No centralized identity verification. The protocol does not rely on centralized ID verification services, which are expensive and can compromise privacy. Instead, individual verifications are done peer-to-peer and stored on a DLT. To strengthen the whole system, some selected users that agree to do so will participate in centralized ID verifications during the initial phase where the network is less mature and lacks local verifications
- No online verification methods. There is no online verification process forseen, as online information can be manipulated or faked, especially with modern AI technology. While this makes the verification process more elaborate, it ensures that the identity verification is reliable and resistant to manipulation. Again, selected individuals might be verified online during the ramp up phase to kick start the network.
- No use of biometric data. Biometric data will not be used due to cost, privacy concerns, and accessibility. Instead, the PeerID protocol requires users to engage in peer-to-peer verifications with people they choose and trust. While this may reduce the ability to automatically identify duplicate profiles and reliability of individual verifications, it allows more users to participate in the service and provide more privacy. Given there are multiple, confirming verification from different peers, a very high verification confidence can be reached that even exceeds biometric methods
- No fees. The service is designed to be cost free for end-users and make it accessible and usefull to all.
- No centralized data. PeerID is designed to run in a decentralised manner using distributed ledger technology. While this makes the system more complex, this is the most suitable way to remove dangerous single points of failures, allow full transparency and build trust among it's users.

While there are trade-offs, PeerID aims to provide the optimal balance in terms of usability, accessibility and privacy while maintaining high, tamper-proof security.
