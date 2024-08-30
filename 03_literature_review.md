# 3. Literature Review

This chapter provides a comprehensive review of existing literature on blockchain-based voting systems, their applications in various contexts, and their potential relevance to Bangladesh's electoral challenges. The review is structured to cover key aspects of blockchain voting, including technological foundations, implementation case studies, security and privacy considerations, and identified research gaps.

## 3.1 Blockchain-Based Voting Systems

### 3.1.1 Technological Foundations

Blockchain technology, originally developed as the underlying mechanism for cryptocurrencies, has emerged as a potential solution for enhancing the integrity and transparency of voting systems (Kshetri & Voas, 2018). The fundamental principles of blockchain technology that make it suitable for voting applications include:

1. **Decentralization**: Unlike traditional centralized voting systems, blockchain-based systems distribute data across multiple nodes, reducing single points of failure and the risk of centralized manipulation (Yavuz et al., 2018).

2. **Immutability**: Once a transaction (vote) is recorded on the blockchain, it becomes extremely difficult to alter or delete, ensuring the integrity of the voting record (Atzori, 2017).

3. **Transparency**: All transactions on a blockchain are visible to all participants, allowing for real-time auditing and verification of the voting process (Noizat, 2015).

4. **Cryptographic Security**: Advanced encryption techniques protect the confidentiality of votes while ensuring their authenticity (Hardwick et al., 2018).

These characteristics address many of the challenges faced by traditional voting systems, particularly in contexts like Bangladesh where trust in the electoral process has been eroded (Rahman, 2019).

### 3.1.2 Architectures and Protocols

Various blockchain architectures and protocols have been proposed for voting systems, each with its own strengths and limitations:

1. **Public Blockchains**: Systems like Follow My Vote use public blockchains like Bitcoin or Ethereum, leveraging their established security and decentralization (Follow My Vote, 2020). However, these systems often face scalability issues and may not provide the level of privacy required for national elections.

2. **Permissioned Blockchains**: Platforms like Hyperledger Fabric offer more control over who can participate in the network, potentially addressing some privacy concerns while maintaining transparency (Ansper et al., 2018).

3. **Hybrid Systems**: Some proposed architectures combine blockchain with other technologies, such as homomorphic encryption or zero-knowledge proofs, to enhance privacy and scalability (Park et al., 2021).

4. **Consensus Mechanisms**: Various consensus protocols have been adapted for voting systems, including Proof of Stake (PoS) and Practical Byzantine Fault Tolerance (PBFT), each offering different trade-offs between security, scalability, and energy efficiency (Wang et al., 2018).

The choice of architecture and protocol significantly impacts the system's performance, security, and suitability for large-scale elections like those in Bangladesh.

### 3.1.3 Smart Contracts in Voting Systems

Smart contracts play a crucial role in automating and securing various aspects of the voting process in blockchain-based systems:

1. **Voter Registration**: Smart contracts can manage voter registration, ensuring that each eligible voter is registered only once and can cast only one vote (McCorry et al., 2017).

2. **Vote Casting**: The actual process of casting a vote can be encoded in a smart contract, ensuring that votes are recorded accurately and immutably (Hardwick et al., 2018).

3. **Vote Counting**: Smart contracts can automate the vote counting process, providing real-time results and reducing the potential for human error or manipulation (Yavuz et al., 2018).

4. **Audit Trail**: Smart contracts can generate a transparent and immutable audit trail of all voting-related activities, enhancing the overall integrity of the election (Atzori, 2017).

The use of smart contracts in voting systems offers significant potential for enhancing the efficiency and transparency of elections in Bangladesh, where manual processes have been prone to errors and manipulation (Riaz, 2020).

## 3.2 Case Studies from Other Countries

### 3.2.1 Estonia's I-Voting System

Estonia has been a pioneer in implementing digital voting systems, including blockchain-based solutions:

- **Implementation**: Estonia introduced internet voting (I-Voting) in 2005 and has been continuously improving the system, incorporating blockchain elements in recent years (Solvak & Vassil, 2018).
- **Technology**: The system uses a combination of public key infrastructure (PKI) for voter authentication and blockchain for vote storage and verification (Kubicek et al., 2016).
- **Outcomes**: I-Voting has been used in multiple elections, with up to 44% of votes cast online in recent elections (Valimised, 2019).
- **Challenges**: Despite its success, the system has faced criticism regarding potential vulnerabilities and the difficulty of ensuring vote secrecy (Springall et al., 2014).

Estonia's experience offers valuable insights for Bangladesh, particularly in terms of gradual implementation and the importance of building public trust in digital voting systems.

### 3.2.2 West Virginia's Mobile Voting Pilot

West Virginia conducted a blockchain-based mobile voting pilot for overseas voters in 2018:

- **Implementation**: The pilot used a mobile app developed by Voatz, which employed blockchain technology for vote storage and verification (Warner, 2018).
- **Technology**: The system used a permissioned blockchain and biometric authentication to ensure voter identity and vote integrity (Voatz, 2020).
- **Outcomes**: The pilot was used in two counties for the 2018 midterm elections, allowing overseas military personnel to vote via smartphone (Warner, 2018).
- **Challenges**: The system faced criticism from security experts regarding potential vulnerabilities and lack of transparency (Specter et al., 2020).

While the scale of this pilot was much smaller than what would be required for Bangladesh's national elections, it provides insights into the challenges of implementing mobile voting solutions in a real-world context.

### 3.2.3 Sierra Leone's Blockchain-Assisted Election

Sierra Leone partially used blockchain technology in its 2018 presidential election:

- **Implementation**: A blockchain-based system was used to record votes in the Western District, alongside the traditional paper-based system (Agora, 2018).
- **Technology**: The system used a permissioned blockchain to create an immutable record of the vote count (Agora, 2018).
- **Outcomes**: While the blockchain system was not used for official results, it provided a parallel record that could be compared with the official count (Agora, 2018).
- **Challenges**: There was some confusion and controversy regarding the extent of blockchain use in the election, highlighting the importance of clear communication in such implementations (Orcutt, 2018).

This case study is particularly relevant for Bangladesh, as it demonstrates how blockchain can be integrated into existing electoral processes in a developing country context.

## 3.3 Security and Privacy Considerations

### 3.3.1 Cryptographic Techniques

Blockchain-based voting systems employ various cryptographic techniques to ensure vote secrecy and integrity:

1. **Homomorphic Encryption**: This allows votes to be counted without decrypting individual ballots, preserving voter privacy (Park et al., 2021).
2. **Zero-Knowledge Proofs**: These enable verification of vote validity without revealing the actual vote content (Cortier et al., 2019).
3. **Ring Signatures**: Used to ensure voter anonymity while still allowing for vote verification (Sun et al., 2017).

The application of these techniques in Bangladesh's context would need to consider the computational resources available and the technical literacy of the voting population.

### 3.3.2 Voter Authentication Mechanisms

Secure voter authentication is crucial for the integrity of blockchain-based voting systems:

1. **Biometric Authentication**: Systems like Voatz use biometric data (e.g., fingerprints, facial recognition) for voter verification (Voatz, 2020).
2. **Multi-Factor Authentication**: Combining something the voter knows (e.g., password), has (e.g., ID card), and is (biometrics) can enhance security (Pawlak et al., 2018).
3. **Blockchain-Based Identity Management**: Some proposed systems use blockchain itself to manage voter identities, potentially reducing the risk of identity theft or fraud (Al-Rawy et al., 2017).

For Bangladesh, where voter list inaccuracies have been a persistent issue (Hassan & Nazneen, 2017), robust authentication mechanisms are particularly important.

### 3.3.3 Resistance to Manipulation and Attacks

Blockchain voting systems must be designed to resist various forms of attacks and manipulation:

1. **Distributed Denial of Service (DDoS) Attacks**: The decentralized nature of blockchain can provide some inherent resistance to DDoS attacks, but additional measures may be necessary (Kshetri & Voas, 2018).
2. **51% Attacks**: In permissioned systems, careful selection of node operators can mitigate the risk of 51% attacks (Wang et al., 2018).
3. **Smart Contract Vulnerabilities**: Rigorous auditing and formal verification of smart contracts are essential to prevent exploitation of code vulnerabilities (Zheng et al., 2020).

Given the history of electoral manipulation in Bangladesh (Moniruzzaman, 2019), designing a system resistant to both technical and social engineering attacks is crucial.

## 3.4 Gaps in Existing Research

### 3.4.1 Scalability Challenges

While blockchain technology has shown promise in small-scale implementations, research on its scalability for national elections in populous countries like Bangladesh is limited:

1. **Transaction Throughput**: Most existing studies focus on small-scale elections or pilots. Research is needed on how to handle the high volume of transactions required for a national election in Bangladesh (Yavuz et al., 2018).
2. **Network Latency**: Studies on minimizing network latency in areas with poor internet infrastructure, which is relevant to many parts of Bangladesh, are lacking (Kshetri & Voas, 2018).
3. **Storage Requirements**: Long-term storage of blockchain data for large-scale elections needs further investigation, especially considering data retention laws and the need for future audits (Zheng et al., 2020).

### 3.4.2 Integration with Existing Electoral Infrastructure

There is a significant research gap in how blockchain-based systems can be integrated with existing electoral processes and infrastructure:

1. **Hybrid Systems**: More research is needed on hybrid systems that combine blockchain with traditional paper-based voting, which could be a transitional solution for countries like Bangladesh (Agora, 2018).
2. **Legacy System Integration**: Studies on integrating blockchain with existing digital systems (e.g., electronic voting machines) are limited (Ansper et al., 2018).
3. **Legal and Regulatory Framework**: Research on adapting legal frameworks to accommodate blockchain voting, particularly in the context of developing countries like Bangladesh, is insufficient (Kouzmin et al., 2019).

### 3.4.3 Socio-Technical Considerations

The social and political implications of implementing blockchain voting systems, especially in contexts like Bangladesh, are understudied:

1. **Digital Divide**: More research is needed on how to implement blockchain voting in areas with low digital literacy and limited access to technology, which is relevant to many parts of Bangladesh (Rahman & Yeasmin, 2020).
2. **Public Trust**: Studies on building and maintaining public trust in blockchain voting systems, particularly in countries with a history of electoral disputes like Bangladesh, are limited (Riaz, 2020).
3. **Accessibility**: Research on making blockchain voting systems accessible to all segments of the population, including people with disabilities and the elderly, is insufficient (Pawlak et al., 2018).

## 3.5 Relevance to Bangladesh's Electoral Context

### 3.5.1 Addressing Voter List Inaccuracies

Blockchain technology has the potential to address the persistent issue of voter list inaccuracies in Bangladesh:

1. **Immutable Voter Registry**: A blockchain-based voter registry could provide an immutable and transparent record of eligible voters, reducing the risk of ghost voters and duplicate entries (Hassan & Nazneen, 2017).
2. **Real-time Updates**: Smart contracts could facilitate real-time updates to the voter list, ensuring it remains current and accurate (McCorry et al., 2017).
3. **Decentralized Verification**: A distributed system could allow for decentralized verification of voter eligibility, potentially reducing the risk of centralized manipulation (Yavuz et al., 2018).

### 3.5.2 Enhancing Transparency and Trust

The transparency inherent in blockchain systems could significantly improve trust in Bangladesh's electoral process:

1. **Immutable Audit Trail**: Blockchain's immutable ledger could provide a transparent and tamper-resistant record of all voting activities, addressing concerns about vote manipulation (Atzori, 2017).
2. **Real-time Monitoring**: Stakeholders could potentially monitor the voting process in real-time, enhancing transparency and reducing the potential for fraud (Noizat, 2015).
3. **Decentralized Control**: By distributing control among multiple stakeholders, blockchain could reduce the risk of centralized manipulation, a significant concern in Bangladesh's elections (Riaz, 2019).

### 3.5.3 Overcoming Infrastructure Limitations

Blockchain technology could potentially address some of the infrastructure challenges faced by Bangladesh's electoral system:

1. **Resilience to Network Issues**: Distributed systems could provide greater resilience to network failures or intentional disruptions, a significant concern in Bangladesh (Kshetri & Voas, 2018).
2. **Reduced Dependence on Physical Infrastructure**: Blockchain-based systems could potentially reduce the reliance on physical voting infrastructure, which has been vulnerable to violence and manipulation in past elections (Human Rights Watch, 2019).
3. **Gradual Implementation**: Blockchain solutions could be implemented gradually, starting with specific aspects of the electoral process (e.g., voter registration) and expanding over time, allowing for a phased approach that considers Bangladesh's infrastructure limitations (Solvak & Vassil, 2018).

In conclusion, while blockchain technology offers promising solutions to many of the challenges faced by Bangladesh's electoral system, significant research gaps remain. Addressing these gaps and carefully considering the unique context of Bangladesh will be crucial for the successful implementation of a blockchain-based voting system in the country.
