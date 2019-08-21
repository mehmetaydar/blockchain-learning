[1 Introduction ](#introduction)

> [**1.1** **What is blockchain?** ](#what-is-blockchain)
>
> [**1.2** **Main technologies constituting blockchain**](#main-technologies-constituting-blockchain)

[**1.2.1** **Cryptography, hashing and digital signature**](#cryptography-hashing-and-digital-signature)

[**1.2.2** **P2P** ](#p2p)

[**1.2.3** **Proof of Work** ](#proof-of-work)

> [**1.3** **Chains of blocks** ](#chains-of-blocks)
>
> [**1.4** **Consensus algorithms** ](#consensus-algorithms)

[**1.4.1** **Proof of Stake (PoS)** ](#proof-of-stake-pos)

[**1.4.2** **Proof of Importance (PoI)** ](#proof-of-importance-poi)

[**1.4.3** **Practical Byzantine Fault Tolerance (PBFT)**](#practical-byzantine-fault-tolerance-pbft)

> [**1.5** **Smart contracts** ](#smart-contracts)
>
> [**1.6** **Major milestones of blockchain**](#major-milestones-of-blockchain)
> 
>[**1.7** **Weakness and Threats of blockchain**](#weakness-and-threats-of-blockchain)

[2 Applications of blockchain ](#applications-of-blockchain)

> [**2.1** **Cryptocurrency & financial services and mobile money**](#cryptocurrency-financial-services-and-mobile-money)
> 
>[**2.2** **Identity management** ](#identity-management)
> 
>[**2.3** **Title & Ownership rights** ](#title-ownership-rights)
> 
>[**2.4** **Supply chains** ](#supply-chains)
> 
>[**2.5** **Sharing economy** ](#sharing-economy)
> 
>[**2.6** **Smart contracts** ](#smart-contracts-1)
> 
>[**2.7** **Blockchain applications for Communication Service Providers
> (CSP)**](#blockchain-applications-for-communication-service-providers-csp)
> 
> [**2.8** **Blockchain in smart cities**](#blockchain-in-smart-cities)

[3 Blockchain consortia ](#blockchain-consortia)

> [**3.1** **Hyperledger** ](#hyperledger)
>
> [**3.2** **R3** ](#r3)
>
> [**3.3** **Ethereum** ](#ethereum)
>
> [**3.4** **Comparison of Hyperledger Fabric, Ethereum, and Corda**](#comparison-of-hyperledger-fabric-ethereum-and-corda)

[4 Company's blockchain activities and interests](#huaweis-blockchain-activities-and-interests)

[4.1 Huawei](#huaweis-blockchain-activities-and-interests)

> [**5.1** **IBM** ](#ibm)
>
> [**5.2** **Cisco** ](#cisco)
>
> [**5.3** **Orange** ](#orange)
>
> [**5.4** **Ericson** ](#ericson)

[6 Blockchain project ideas ](#blockchain-project-ideas)

> [**6.1** **Identity management via blockchain**](#identity-management-via-blockchain)
> 
>[**6.2** **Extending IDaaS for digital documents management and record
> verification:**](#extending-idaas-for-digital-documents-management-and-record-verification)
> 
> [**6.3** **Blockchain for Electronic Health Records (EHR)**](#blockchain-for-electronic-health-records-ehr)
>
> [**6.4** **Transparency in the supply chain in Agriculture**](#transparency-in-the-supply-chain-in-agriculture)
> 
>[**6.5** **Other possible implementations**](#other-possible-implementations)

[7 References ](#references)

Introduction
============

Blockchain is a technology that provides secure immutable transfer of
value based on distributed ledger technology. Blockchain eliminates the
necessities of trusted third parties by embedding Trust Fabric into its
very nature. Therefore, **it disrupts the sectors and services that need
intermediaries, such as** banks, insurance services, supply chains, etc.

Blockchain is the backbone of the Bitcoin cryptocurrency, which was
**created in 2008 to transfer financial value within the context of the
peer-to-peer currency**. Ten years after the blockchain was invented,
there is a shift in focus from the cryptocurrencies towards the core
elements of the blockchain itself and how its nature as a distributed
ledger for transactions could be leveraged.

Historically, it has proven that Blockchain ensures no downtime, make
falsification extremely hard, inexpensive to implement and provides
privacy and data integrity. Therefore it creates innovative business
logics and interesting research areas.

**Banks, governments, information & communication technology companies
and companies in variety of sectors are looking for potential
opportunities about how they can use blockchain technology in new
application areas such as property transfers, identity services, and
data management. Although it** has some way to go before the technology
will reach a mainstream adoption, **blockchain technology will
definitely disrupt areas in which many sectors currently do business.
Therefore it is vital to begin studying its impact and experimenting
with its future possibilities.**

**What is blockchain?**
-----------------------

Blockchain is a distributed database that stores a permanent and
tamper-proof record of continually updated list of transactions. Unlike
traditional databases, distributed ledgers are managed through a
peer-to-peer (P2P) architecture, but the final decision is made through
a consensus among the nodes. Blockchains are most commonly associated
with cryptocurrency, Bitcoin in particular.

A blockchain ledger consists of transactions and blocks. A transaction
is a "value transfer" between two participating nodes, i.e. sending a
financial asset. The end user\'s software creates a hash of the
information in each block and stores the hash with the block that is
currently at the end of the blockchain. The hash of the previous
block\'s data is also included in the new hash that is stored at the end
of the blockchain. This inclusion makes tampering with blockchain data
practically impossible. Altering any transaction in a block changes the
block's hash and makes subsequent hashes associated with the following
blocks incorrect. This is important because when a hashing function is
run on a block to check its validity and the hash does not match the
stored value, it means the record has been tampered with or is otherwise
corrupt. Legitimate changes to the ledger are recorded across the
blockchain in a matter of minutes or seconds and records are protected
through cryptography.

**In simple terms, blockchain can be thought as a book, where each page
of the book corresponds to an individual block and each paragraph in a
page corresponds to an individual transaction. The paragraphs
(transactions) in each page (block) are hashed, allowing the page
(block) to be represented with one single hash value. Each page (block)
references the previous page (block) by its hash. That is called chain.
In this sense, the book (blockchain) mimics the behavioral of a singly
linked list data structure, where the header element of the linked list
is the last page (block) in the book (blockchain).**

**The book (blockchain) itself can be called a ledger, and the same and
up to date copy of the book is distributed and kept by many parties
(distributed ledger). When records are added they are appended as a new
page to the book, and each party (node) updates their copy of the book
(blockchain) accordingly. The new pages (blocks) cannot be added
randomly, it is rather decided by a powerful consensus algorithm between
the parties (nodes). The records cannot be altered due to each block
references to the previous block. So to alter one block all the
subsequent blocks have to be altered. Even if a hacker did that, they
only altered their portion or small portion of the whole distributed
database. They need to alter at least 51% of the whole distributed
database to be verified. This needs immense machine power and is
impractical.**

**To summarize,**

-   Blockchain is basically a database, with the difference that it is
    decentralized and distributed, existing on millions of nodes.

-   Blockchain takes account of the past, and the past is public.
    Anything ever taken place in the database is permanently saved, and
    anyone can track any change back to the origin.

-   Blockchain provides secure immutable transfer of value. It leads the
    revolution of the internet from the internet of things to internet
    of value.

-   The core attributes of Blockchain's shared ledger approach
    contributes providing trust, security, transparency and control
    across the participating ecosystem for all points in a transaction
    process. This results in the potential for lower costs and improved
    experiences for all players.

**Main technologies constituting blockchain**
---------------------------------------------

Blockchain is considered to have created new functions by combining
existing technologies. Major technologies constituting blockchain (hash,
public-key cryptography, digital signature, P2P and Proof of Work) are
outlined below.

### **Cryptography, hashing and digital signature**

The science of encrypting and decrypting messages (cryptography) has
been used for thousands of years. Asymmetric cryptography or public-key
cryptography is a cryptographic method using different keys for
encryption and decryption. The problem of handing over keys was solved
by dividing the key into one for private use (private key) and one
available for anyone (public key). Public-key cryptography enables safe
delivery and receipt of files only if a receiver prepares a pair of a
private key and a public key and delivers the public key to the sender
in advance. Safety can be maintained even though other persons use the
public key as long as the receiver properly manages his/her private key.

![](media/image1.png)

> Figure 1 - Mechanism of public-key cryptography

Hashing is generating a value or values from a string of text using a
mathematical function. It is extremely difficult to infer the original
data based on a hash value. Blockchain system takes advantage of such
characteristics for the verification and guarantee of the continuity of
block data and the creation of blockchains through consensus algorithms.

> Table 1- Sample sha1 hash

![](media/image2.png)

A digital signature refers to a mechanism to prove the authenticity of
the data sent via a network and a pair of keys used in public-key
cryptography is also used here. Generally, a digital signature, which is
made by encrypting the hash value of a file to be sent to a receiver
with the sender's private key, is sent to the receiver together with
said file. The receiver uses the same hash function as the sender to
create the hash value of the file by him/herself and cross-checks the
created hash value with the hash value obtained through decrypting the
sender's digital signature with the sender's public key, thereby
confirming that the sender's digital signature is authentic. For
instance, In the Bitcoin system, public-key cryptography and a digital
signature are used for identifying a creator of transaction data (data
of a Bitcoin transaction) and as an address of a Bitcoin wallet. The
encryption method used in Bitcoin is SHA256 which was originally
designed by United States National Security Agency (NSA). SHA256 is also
being used for decades in many sectors and services that requires solid
security, i.e. in financial services, and it has proven to be secure
(Institute, 2016).

![](media/image3.png)

> Figure 2 - Example of digital signature (What Is a Digital Signature?,
> 2018)

### **P2P**

In a P2P network, all participating nodes (referring to computers for
communication; also called "peers" or "nodes") hold data respectively
and create an autonomous network wherein data are requested and provided
among these nodes on an equal footing. In a P2P network, roles of
respective nodes as a server or a client are not fixed, unlike the case
of a client-server network. P2P networking technology has contributed to
developing a base for a complete distributed network and eliminating
single point of failure in Blockchain (Institute, 2016).

### **Proof of Work**

Proof of Work (POW), is a consensus algorithm, generally refers to a
mechanism to confirm a person's innocence by having him/her do a certain
work. POW is a work called mining in Bitcoin. Network participants
calculate a hash value by adding a nonce (any given value) to the
collection of transaction data delivered to them. It is required to
obtain a value smaller than a certain value, and the participants have
to continue calculations by using different nonces until they obtain the
value as required. The formula is as below:

> **Hash** (*Prev\_hash,* *Tx\_Root,* *Timestamp,* *Nonce*) \<
> **Difficulty**

Difficulty is a value used to show how hard it is to find a hash that
will be lower than target defined by system. In case of Bitcoin,
difficulty increases in every 2016 blocks, and that is why mining gets
harder in time. When the first Bitcoin block (called genesis block) is
mined in 2009 the difficulty was 1. As of June 08 2018 the difficulty is
4,940,704,885,521.

When anybody obtains the relevant value, network participants mutually
confirm the correctness of the value and the collection of transaction
data used for the calculations is approved to be official transaction
results as a new block.

Then, coins are granted as a reward to the person who succeeded in
obtaining the correct value through the calculations. After that, all
participants go on to the next mining using transaction data that were
not included in said block and the newly created transaction data.
Bitcoin employs PoW to create a mechanism that can prevent falsification
of data and duplicate payments without a central authority and can
maintain the system against any attacks by malicious users.

![](media/image4.png)

> Figure 3 - Calculating nonce value (mining) (Institute, 2016)

**Chains of blocks**
--------------------

A block of one or more new transactions is collected into the
transaction data part of a block. Copies of each transaction are hashed,
and the hashes are then paired, hashed, paired again, and hashed again
until a single hash remains - the merkle root of a merkle tree. This is
illustrated below:

![](media/image5.png)

Figure 4 - Merkle tree (Technologies, 2017)

4f68594945ccded4d77a01992db7f4c5 is the merkle root of the 4
transactions (or pieces of data) in the illustration above. This is
stored in the block header. Additionally, each block also stores a
timestamp, a nonce value and the hash of the header of the previous
block. This chains the blocks together and ensures that a transaction
cannot be modified without modifying the block that records it and all
following blocks (Ltd., 2017). Transactions are also chained together.
This is illustrated below:

![](media/image6.png)

Figure 5 -- Example blockchain blocks (Technologies, 2017)

In case of Bitcoin, blocks are generated in approximately 10 minutes.
The number of Bitcoins generated per block starts at 50 and is halved
every 210,000 blocks (about four years). As of June 08 2018, 526527
number of blocks are mined.

**Consensus algorithms**
------------------------

In blockchain, all participants must agree on new block creation and
that a transaction is valid. This is called consensus. For Bitcoin, the
Proof of Work consensus algorithm is used as explained above. PoW
requires a lot of machine power and as a result it consumes
significantly more electricity. As a matter of the fact, blockchain
developers researched and implemented other alternatives.

### **Proof of Stake (PoS)**

PoS refers to a method to assign priority in hash calculations, in
accordance with the holding ratio of virtual currency, etc. This is
based on the idea that a dishonest act committed by a node holding a
large amount of virtual currency results in reducing the reliability and
value of the currency and this fact works as an incentive for any
participant to avoid dishonest acts. However, several means to illegally
control blockchains are pointed out and countermeasures are necessary.
PoS is adopted in Ethereum, Bitshares, and NXT, cryptocurrencies
(Institute, 2016).

### **Proof of Importance (PoI)**

PoI refers to a method to cluster nodes through transaction graph
analysis using transaction amounts and balances of individual nodes as
indicators, calculate the significance of each node, and assign priority
in hash calculations (assign easier hash calculations) to more
significant nodes. Clustering is supposed to make it possible to detect
nodes that are likely to commit unlawful transactions. PoI is adopted in
NEM cryptocurrency (Institute, 2016).

### **Practical Byzantine Fault Tolerance (PBFT)**

PBFT is an algorithm for solving a Byzantine Fault resulting from a
failure in building a consensus caused by the Byzantine Generals
Problem. It was considered to be difficult to put a theoretical
algorithm to practical use due to the enormous calculation amount being
required. In 1999, a practical algorithm that can avoid a Byzantine
Fault by adding a minor lag at the time of judging consensus formation
was propounded, and efforts to apply this algorithm to blockchains are
made. However, the total number of nodes must be known and the maximum
number of illegal nodes should be set, and such requirements make it
difficult to apply this algorithm to public systems. PBFT is adopted in
Ripple and Stellar, also in Hyperledger Fabric (Institute, 2016).

**Smart contracts**
-------------------

Blockchain based smart contracts, a feature not available in all
Blockchain platforms, are self-executing code that automatically
implement the terms of an agreement between two or more parties. This
offers a number of benefits including;

-   real or near real-time updates,

-   accuracy by being less prone to human errors,

-   lower contract execution risk by eliminating manipulation and
    non-performance,

-   fewer intermediaries by removing reliance on third-parties such as
    escrow services,

-   lower cost since it requires less human intervention and fewer
    intermediaries, and

-   Promoting new business and operational models by allowing peer to
    peer trading in traditionally legacy industries such as renewable
    energy.

An example to the usage of smart contracts can be seen in the music and
entertainment industry. Smart contracts can improve the manner in which
revenue flows from consumer to artist or content creator, and reduce
reliance on collecting and managing statistics to distribute royalties.

The new generation blockchain networks such as Ethereum, Neo, and
Hyperledger Fabric have smart contract capabilities. Smart contracts
provides an application layer that run on the blockchain network.

**Major milestones of blockchain**
----------------------------------

Blockchain has earned a tremendous attention from both industry and
research community after Bitcoin's mysterious inventor Satoshi Nakamoto
published the research paper titled as "Bitcoin: Peer-to-Peer Electronic
Cash System" in 2008 (Nakamoto, 2009). The paper detailed methods of
using a peer-to-peer network to generate what was described as \"a
system for electronic transactions without relying on trust. On the of
3rd January 2009, the Bitcoin network came into existence with Satoshi
Nakamoto mining the genesis block of Bitcoin (block number 0), which had
a reward of 50 Bitcoins. The real identity of Satoshi Nakamoto remains
secret. However no doubt that he/she/they/it presented a revolutionary
system for peer to peer transactions, eliminating trusted third parties
but still guaranteeing trust among the peers.

The figure above shows the major milestones of blockchain. It is
expected that between 2018 and 2020 consortium will be instrumental in
defining protocols and common standards, and regulatory bodies will play
a pivotal role in ensuring compliance. Also by 2020 and beyond,
blockchain will gain adoption across various industries leading to new
business models. For instance, it is expected that blockchain will be
storing over 10% of the global GDP by 2027 (Forum, 2015).

**Weakness and Threats of blockchain**
--------------------------------------

Blockchain brings revolutionary benefits to many services and
industries. However, it is still immature. It has scalability issues. It
needs to have protocols and standards set. Bitcoin mining requires
immense power consumption.

Applications of blockchain
==========================

Blockchain cannot solve all the problems in all the sectors, but it
solves a lot of problems in a lot of sectors. Trust is the primary
driver of blockchain. The application that requires trust, authenticity,
immutability and traceability can benefit most from blockchain. In
another words, blockchain is beneficial most to the industries and
application where trust among the parties is low but trust, security and
integrity is a must. In this section, some example use cases of
blockchain is explained.

**Cryptocurrency & financial services and mobile money**
--------------------------------------------------------

Bitcoin is the first cryptocurrency in the blockchain history. With
cryptocurrency, peers can transfer money securely, fast, easily with
minimum transaction fee. This disrupts financial and telecommunication
industries as both provide money transfer.

It is possible to distribute and manage local currency issued by a local
government or by a company, etc. on a blockchain. Local currency is
issued to residents or customers through certain procedures and is used
at stores within the relevant community or for payments for public
services, etc. Similar services include (Institute, 2016):

-   **Remittance**: Blockchains may be used for sending and receiving
    all value information including local currency and various types of
    virtual currency, not limited to remittance of legal currency. If a
    public-type blockchain is adopted, such remittance service naturally
    covers the whole world.

-   **Loyalty point services**: Companies can provide their loyalty
    point services on blockchains. If exchange of different types of
    loyalty points is made possible among users, the advantage of
    utilizing blockchains will become larger.

**Identity management**
-----------------------

Traditional identity management methods are open and susceptible to
identity theft and fraud. It requires the need for integrating various
silo systems. Different parties have to verify your identity using
different form of identity copies. With blockchain your identity can be
stored once in Blockchain and can be verified by all the parties. Once
your ID is stored in Blockchain it is there and can only be viewed by
the parties who have permission. Microsoft has some early plans to start
producing identity documents as an alternative to identity documents
issued from nations. IBM also has a similar vision.

**Title & Ownership rights**
----------------------------

Tracking ownership of physical and non-physical property, such as cars,
real estate, stocks, and other assets can be run on a Blockchain
platform. Huawei has a use case on this where the digital property
rights are kept in Blockchain and access to the properties are managed
by smart contracts (coininsider, 2016).

A convenient example would be land registration, in which it is possible
to register, publicize, and manage information on land, such as physical
status and related rights, on blockchains. Not only data on land,
buildings, and owners, but also the transfer of land or other property
and the establishment of a mortgage may be recorded and managed and this
will improve the efficiency of related operational work. Information on
land and buildings and records of transfer thereof can be managed.
Additionally, information on the division and consolidation of land
(parcel subdivision and parcel consolidation), as well as on ownership
and mortgages or other related rights that is now managed on registries
may also be managed on blockchains. Such information will be made
available for inspection to anyone in the same manner as in the case of
the current registries (Institute, 2016). Similar applications include:

-   **Patent information**: Patent and copyright related information may
    also be managed on blockchains. If not only the details of patents
    but also their ownership are managed on blockchains, the management
    of transactions of rights may also become possible on blockchains.
    Blockchain "hashing" and "proof of existence" (verifying that a
    digital content existed at a certain point in time) also make the
    technology helpful in improving the patent system, particularly
    where there is no unified patent systems across countries.
    Blockchain technology could make patent systems more efficient and
    provide more economical proof of existence services.

-   **Electronic health records**: Personal medical data may also be
    managed on blockchains. Consistent medical treatment at multiple
    hospitals may become available with a due consideration to privacy
    by limiting information managed on blockchains to only records of
    individuals' hospital visits, while having respective hospitals
    manage details of their patients' health records.

-   **Various notifications** (notifications of birth, change of
    address, marriage, etc.): Mainly various notifications to local
    governments may be managed on blockchains. For example, if the
    resident register is managed on a blockchain, a notification of
    change of address may be completed only with digital signatures of
    the relevant person and the local governments before and after the
    moving.

-   **Voting**: Voting rights may also be managed on blockchains. (As
    long as digital signatures are safely managed) double voting can be
    avoided. As an example, Follow My Vote (followmyvote, 2018), a
    company from Virginia, is building an on-line platform for voters to
    cast their vote in an election via the smart phone.

**Supply chains**
-----------------

Blockchain provides transparency. This will disrupt traditional value
chain services such as supply chain management. Production process of
products starting from raw materials, as well as their distribution and
sale may be traced on blockchains. Trade records (receipt and placement
of orders, estimated delivery dates, etc.), processing records of
processed goods, identification data of individual goods (lot number and
specifications), information to guarantee authenticity, and the process
from manufacturing to distribution of industrial products, etc. may all
managed on blockchains (Institute, 2016). Similar applications include:

-   **Management of precious metals and jewels**: Utilization of
    blockchains for managing each piece of precious metals and jewels,
    such as gold and diamonds, from their processing stages will enable
    purchasers to check the processing records of products and this may
    increase credibility of products. For instance, (Lomas, 2015) is a
    global startup from UK that keeps track of diamond's every movement
    in the distribution channel via a chain of digital certifications.

-   **Certification of authenticity of works of art, and others**: If
    works of art and artifacts with their creators' signatures are
    managed using blockchains, their authenticity can be confirmed even
    after being circulated in the market and copyright management will
    become easier, which may decrease counterfeits of works of art. As a
    result, blockchain technology can assist in identifying copyrighted
    works and settling disputes, leading to better licensing policies
    and improved legal certainty for creators and consumers of content.

**Sharing economy**
-------------------

The business structure of AirBnB and Uber are example of sharing economy
where people pay for the services and assets they rent. Information on
transfer of rights to use of assets, etc. and evaluations by providers
and users may be recorded on blockchains. Information on holders of
rights to use of assets to be shared, as well as information on transfer
of such rights and payments and receipts of money is to be mainly
managed on blockchain. Evaluations by providers and users may also be
managed (Institute, 2016). Similar applications include:

-   **Electronic libraries and digital contents**: By using blockchains
    for the management of rights to read electronic books, electronic
    libraries may be realized. In a similar manner to the case of
    electronic libraries mentioned above, rights to use digital contents
    can be managed by blockchains. This may promote use of digital
    contents while protecting copyright holders.

-   **Smart locks and smart sockets**: Diverse usage of blockchains in
    daily lives can be considered, for applications such as for managing
    the authority to unlock a key or the authority to use electricity by
    plugging an appliance into a socket. New business models for using
    blockchains for these purposes to provide sharing services may be
    developed.

**Smart contracts**
-------------------

The idea of a smart contract was already propounded in the 1990s, but
emergence of blockchains has made it achievable without the involvement
of third parties. Smart contracts are self-executing code that
automatically implement the term of an agreement between two or more
parties. It has a lot of potential benefits. It promotes new business
and operation models by allowing peer to peer trading in traditionally
legacy industries such as renewable energy. Contract terms, performed
obligations, various procedures, work processes and future processes,
etc. may be recorded on blockchains (Institute, 2016).

-   **Derivatives (derivative financial instruments):** In derivative
    transactions, funds are paid and received under various conditions.
    If such conditions are determined in advance under a smart contract,
    automatic judgment of satisfaction of conditions and settlement
    processing may become possible.

-   **Escrow service**: A smart contract system on a blockchain may
    eliminate the need for third party intermediaries in transactions
    and thereby realize an escrow service.

-   **Energy control**: A smart contract system may enable automatic
    battery charging for electric appliances (home appliances and
    electric vehicles, etc.) connected to blockchains depending on their
    utilization status, and automatic settlements by predetermined
    means.

-   **Company liquidation**: A smart contract system may enable
    automatic allocation of assets or various rights in the event of
    company liquidation.

**Blockchain applications for Communication Service Providers (CSP)**
---------------------------------------------------------------------

> Blockchain can provide the following benefits for Communication
> Service Providers (Deloitte, 2018):

-   A blockchain's 'enabled' trust improves coordination between various
    partners, due to a shared view of transactions and liabilities. This
    in turn permits the elimination of third parties, resulting in cost
    savings.

-   Facilitates a single view of data instead of the need for
    consolidation across various disparate systems. Also allows for
    reliable audit trails due to the history of all transactions being
    available in the ledger.

-   Implementation of smart contracts in roaming and other cases allows
    for near-instantaneous charging, thus leading to improved revenue
    assurance and fraud reduction.

-   Potential to facilitate new business models for revenue generation
    for Communication Service Provider who are looking for new avenues
    to increase both top and bottom lines.

-   A blockchain can act as the ledger that enables, for example, an M2M
    economy to prosper based on the common platform available, in which
    M2M transactions can be recorded. It can thus act as the enabler for
    an IoT ecosystem.

Below are some use cases:

-   Prevent roaming fraud

-   Prevent subscription identify fraud

-   Provide identity-as-a-service

-   Provide data storage and verification services to private clients,
    i.e. verifying if a subscriber did completed a certification from a
    University.

**Blockchain in smart cities**
------------------------------

Blockchain technologies have a lot of potential use cases in the era of
smart cities. Some of the blockchain applications are explained below
(Diender, 2017):

-   **Healthcare:** Secure exchange of value between all the parties
    involved. (Patients, doctors, pharmacies, event machines).

-   **Government:** eGovernment platforms can be linked to different
    information systems using blockchain to exchange valuable
    information.

-   **Education:** Blockchain can be applied to online exams by securing
    the integrity of the answers between the students and teachers. Can
    also be applied to payment of tuition, accessing digital libraries
    etc.

-   **Library:** Blockchain can be applied to locate the library
    resources such as books, the movements of books. Can help locating
    the books. Similar to supply chain transparency.

-   **Transportation:** Blockchain can be applied for the automatic
    payment of speeding tickets, road taxes, and toll fees. With a
    blockchain implementation the cars will be connected via a
    blockchain network. Blockchain will facilitate the secure exchange
    of safety-critical data between trusted terminals and endpoints.

-   **Public safety:** Blockchain can facilitate the secure and safe
    exchange of information required. It will eliminate 3^rd^ party
    solutions to achieve end-to-end security.

Blockchain consortia
====================

The current Blockchain ecosystem is still immature. However several consortia are working on building Blockchain technologies, creating proofs of concepts, and promoting their technologies.  
----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Many large companies, have joined one or more of these
consortia to establish standards and best practices for a more mature
technology with better adoption rates in industries outside the Banking
and Financial Services Industry.

**Hyperledger** 
----------------

Hyperledger is an open source initiative by The Linux Foundation that
aims to create common open source Blockchain frameworks and tools that
anyone can download and take into use, with just under 190 members from
a diverse range of backgrounds and industries including banking,
technology, consulting, retail, governments, academia among others.
Consultancies, Banks, Government entities (like Smart Dubai).

*Fabric is Hyperledger's most active project. Initiated by IBM.
Foundation for developing blockchain distributed ledger applications
with a modular architecture. It allows components, such as consensus and
membership services. It can be thought as granddaddy. Core platform is
written in Go. It also supports Java. It allow private channels. Which
means you can select the parties you want to share your data privately
on a large network. This is the most distinctive feature about Fabric.
Hyperledger* Sawtooth is originally developed by Intel. Consensus is
based on Proof of Elapsed time which targets large distributed validator
populations with minimal resource consumption (less Cpu or Gpu work)
*(Hyperledger, 2018).*

Hyperledger Caliper is a blockchain benchmark tool to test the
performance of major blockchains. It is initially developed by
developers from Huawei, Hyperchain, Oracle, Bitwise, Soramitsu, IBM and
the Budapest University of Technology and Economics. Hyperledger Caliper
allows users to measure the performance of a specific blockchain
implementation with a set of predefined use cases, and will produce
reports containing a number of performance indicators such as success
rate, throughput, latency and resource consumption (Hyperledger Caliper,
2018).

**R3** 
-------

R3 is a distributed database technology company, which leads a
consortium of more than 200 firms in research and development of
distributed ledger usage in the financial system and other areas of
commerce. R3, together with some of the world's largest financial
institutions, and manufactures has created a Blockchain platform called
Corda, targeted specifically for financial markets. Corda allows network
participants to manage financial agreements in a DLT bypassing the
complexities of silo systems and platforms (r3, 2018).

**Ethereum**
------------

Ethereum is an open software platform based on blockchain technology
that enables developers to build and deploy decentralized
applications. Ethereum blockchain focuses on running the programming
code of any decentralized application. The decentralized application in
Ethereum is written in a specialized Turing-complete programming
language called Solidity.

Quorum is an enterprise-focused version of Ethereum supported by J.P.
Morgan. Quorum is ideal for application requiring high speed and high
throughput processing of private transactions within
a permissioned group of known participants. Quorum addresses specific
challenges to blockchain technology adoption within the financial
industry.

The Enterprise Ethereum Alliance (EEA) probably the largest Blockchain
initiatives, now 220+ members in its consortium, is focused on advancing
Ethereum based Blockchain solutions in the market, and companies like
Microsoft, MasterCard, J.P. Morgan, Santander, Cisco and UBS are active
member in this consortium.

**Comparison of Hyperledger Fabric, Ethereum, and Corda**
---------------------------------------------------------

Hyperledger Fabric and Ethereum both are highly flexible, but in
different aspects. Ethereum's powerful smart contracts engine makes it a
generic platform for literally any kind of application. However,
Ethereum's permissionless mode of operation and its total transparency
comes at the cost of performance scalability and privacy. Fabric solves
performance scalability and privacy issues by permissioned mode of
operation and specifically by using a BFT (Byzantine Fault Tolerance)
algorithm and fine-grained access control. Further, the modular
architecture allows Fabric to be customized to a multitude of
applications. An analogy to a versatile toolbox can be drawn.

Corda is located at the other end. It has been consciously designed as
distributed ledger technology (DLT) for the financial services industry.
Most notably, it takes the highly regulated environment into account by
augmenting smart contracts with legal prose. Corda's focus solely on
financial services transactions simplified its architectural design
compared to Fabric. Therefore, it might offer a more out-of-the-box
experience. However, it might be possible that Fabric, due to its
modularity, can be tailored to resemble Corda's feature set. Efforts
exist that seek to integrate Corda into the Hyperledger project. Corda
therefore cannot be seen as a competitor to Fabric but more as a
complement (Martin Valenta, 2017).

> Table 2 - Comparison of Ethereum, Fabric and Corda (Martin Valenta,
> 2017)

![](media/image9.png)

Company's blockchain activities and interests
============================================

**HUAWEI**

> Blockchain is an enabler for Huawei's strategy of fueling digital
> transformation through "pipe-device-cloud." It also introduces new
> business models and revenue streams. In February 2017, a
> cross-departmental joint workgroup was appointed in Huawei with the
> objective of "formulating the company's unified Blockchain business
> strategy and marketing plan". In December 2017, the group identified
> several use cases. In January 2018 the group finalized the strategy:
>
> One example use case is charity donations. Assuring the funds being
>requested are legitimate foundations and donors know that their
> donations are going toward the cause they want.
>
> 

Huawei is a member of Hyperledger blockchain consortium since October
2016. Huawei is also an early adopters of Hyperledger's sawtooth
software, for which the company is currently developing a decompiler.
Huawei also contributed to the development of Hyperledger Caliper, a
benchmark tool to test the performance of blockchain networks
(Hyperledger Caliper, 2018).

Huawei is also a member of R3 consortium and Huawei financial services
is looking for possibilities to adopt Corda since Corda is specifically
designed for financial services (Huawei IT Solution Forum, 2018).

Huawei launched a blockchain-as-service (BaaS) cloud platform based on
Hyperledger Fabric 1.0. The service enables companies to develop smart
contracts on top of a distributed ledger network for several use-case
scenarios. The use case topics include supply chain, tokenized
securities assets and public services such as ID verification and
financial auditing (Huawei, 2017).

Huawei applied a patent for Blockchain rights management in 2018. The
company detailed an invention that adds a verification feature to a
peer-to-peer content distribution network powered by blockchain tech.
the system would store verification for digital content on blockchain.
When parties initiates download requests over a peer-to-peer network the
system matches their private key or licenses for accessing the content
with the verification information. It is a way to guard intellectual
property rights for digital content that is distributed over P2P network
(Zhao, 2018).

BTC.com's Bitcoin wallet will be pre-installed on all new Huawei's
smartphones, according to Alejandro de la Torre, vice president of
business operations at BTC.com (Alexandre, 2018). There is also an
ongoing negotiations between Huawei and Sirin Labs for developing a
Huawei mobile phone using Sirin Lab's operating system, which is capable
of running blockchain applications alongside android (Davenport, 2018).

**IBM**
-------

IBM is possibly the strongest player in blockchain industry. IBM is the
Initiator of Hyperledger Fabric project. The firm has extensive list of
clients. IBM Established a blockchain business unit in 2016 and
incorporated it into AI and cloud computing. They have BaaS offering.
IBM blockchain platform is built on Hyperledger. Their platform includes
preconfigured use cases for supply chain, financial services,
automotive, real estate, food safety, identity, and international trade
for developers to use.

**Cisco**
---------

Cisco announced trusted IoT alliance consortia focused on
blockchain-enabled, trusted internet of things. The mission is to
develop standards, publishing open source code in blockchain-enabled IoT
to create a trusted IoT ecosystem that links cryptographic and
registrant identities, along with metadata, to give objects equivalent
of digital, transferable birth certificates that can be inventoried and
managed across blockchain networks. They published a common API to
register things to both Hyperledger and Ethereum. They also published a
patent application: blockchain based IoT device identity verification
and anomaly detection.

**Orange**
----------

Orange created a program called ChainForce aims to bring collaboration
on use cases to unlock new opportunities in blockchain. Orange provides
services in verify provenance of physical objects or identity, IoT
identity and smart contracts, etc. They created a company called Chain
which focuses on enablement, creation, management and transfer of
digital assets through blockchain technology, and development of the use
cases in Telecommunication industry.

**Ericson**
-----------

Ericson has a niche blockchain application for organization that work
with critical, sensitive or regulated data, such as those deal in
energy, healthcare, transportation where a serious of data failure could
be catastrophic. They crated Ericson Data Centric Security, uses keyless
signature infrastructure (KSI) blockchain technology built with
Ericson's infrastructure to provide real time massive scale data
integrity validation, time stamping, and signature identification
services allowing organizations to solve difficult security, commercial
and governance problems using a blockchain via distributed computing and
smart contracts.

Blockchain project ideas
========================

**Identity management via blockchain**
--------------------------------------

As an individual you identify yourself using various identity
information such as your age, address, name, and so on. Your identity
verification method can be in the form of driving license, passport,
insurance card, etc. Your identity information are being stored in many
centralized data silos, which hackers are constantly trying to hack.
Traditional identity management methods are open and susceptible to
identity theft and fraud. For business workflow, traditional identity
management methods require the need of integrating various silo systems.
Different parties have to verify your identity using different form of
identity copies.

Digital ID, secure payment, EHR (electronic health records), and KYC
(knowing your customers) are all use cases for digital identity
management. The driving force for the individuals is that you want to
control who has access to your identity record. And for businesses it
means more automated and optimized process workflow.

With blockchain your identity can be stored once in Blockchain and can
be verified by all the parties. Once your ID is stored in Blockchain it
is there and can only be viewed by the parties who have permission.
Microsoft has some early plan to start producing identity documents --
as an alternative to identity documents issued from nations. IBM also
has a similar vision.

We can implement an identity management system using blockchain. A
blockchain can be used as the shared ledger that stores identity
transactions. CSPs (such as Turkcell, Vodafone, and
Turk Telekom) are our potential customers. The CSP can provide
identity-as-a-service to partners, thus allowing for additional revenue
generation by negotiating appropriate agreements.

Deloitte has a similar use case for IDaaS. The system consists of 3
major parts: ID Creation, ID Authentication and Data Management
(Deloitte, 2018).

![](media/image12.png)

> Figure 10 - Deloitte\'s use case for ID creation

Figure 10 shows Deloitte's use cases for ID creation. When a subscriber
opens an account with a CSP, the CSP creates a digital identity with a
public and private key. The private key associated with this identity is
stored safely on the eSIM. The CSP creates a virtual identity, using the
public key from the digital identity and adds a set of standard fields
(name, address, etc.) as required. It then adds a digital signature
using its own private key. A pointer to this virtual identity along with
necessary descriptors is then added to the blockchain (Deloitte, 2018).

![](media/image13.png)

> Figure 11 - Deloitte\'s use case for ID Authentication

Figure 11 shows Deloitte's use cases for ID authentication. If the
subscriber now visits a partner website, say an e-commerce site, the
site will need to know their identity, so the merchant site starts
running the corresponding app on the phone to provide the identity. A
copy of the ledger entry is sent to the e-commerce site app. Now the
e-commerce app can look at all entries for that same virtual identity.
Once the virtual identity is established, the e-commerce site needs to
know that the virtual identity belongs to the subscriber so its app
takes the public key from the virtual identity, encrypts a challenge and
sends it to their app which decrypts it (because it has the associated
private key) and responds. Now the e-commerce site generates an
e-commerce virtual identity which is then stored in the ledger itself.
The next time the subscriber visits the same e-commerce site, he can be
authenticated using the same mechanism. Also, the ledger already holds
his transaction history and hence knows his preferences. The e-commerce
site can use related insights for a recommendation engine. The
subscriber can also use the same e-commerce virtual identity to login to
a completely different e-commerce site using the same mechanism
(Deloitte, 2018).

**Extending IDaaS for digital documents management and record verification:**
-----------------------------------------------------------------------------

The IDaaS use case explained can be extended for digital documents
management and record verification. This adds a powerful feature as it
removes institutional and international boundaries for notarizing
records.

![](media/image14.png)

> Figure 12 - Deloitte\'s use case for Data Management

Figure 12 shows Deloitte's use cases for Data Management part which is
an extension to the IDaaS use case. Consider the example of an
educational institution. Educational institutions issue certificates and
degrees to their students to signal the completion of a course. The
current system of managing certificates is slow, unreliable, and
disjointed. It often still requires maintaining a paper copy of the
certificate to be physically submitted to third parties legitimately
requesting proof of course completion and grades. Additional steps today
might include an employer, for example, calling a university to verify
that a certificate is not a fake, or relying on a third-party to perform
that verification. CSPs could provide blockchain based Identity
verification, data management and storage services to both private
clients and subscribers, generating additional revenue in the process.
The educational institution signs up with the CSP to digitize and store
certificates of subscribers on the blockchain. For those subscribers who
also sign up (and are, of course, alumni of the university), their
identity and degree certificate are verified by the university through
traditional channels, and the university assigns the digital copy of
that certificate along with all details (course name, date of issue,
etc.) to the subscriber. If a prospective employer of the subscriber now
wants to verify the credentials and inspect the certificate, the
subscriber only needs to produce the digital certificate available on
the blockchain and the employer can be sure that this has been issued by
the university and is genuine. The CSP can further benefit by extending
related authentication services to corporate clients for all types of
documents, such as insurance certificates, airline tickets, hotel
reservations, etc., where digital storage and verification may be
required at some point (Deloitte, 2018).

**Blockchain for Electronic Health Records (EHR)**
--------------------------------------------------

When you go to a doctor they ask you about your demographic records,
what previous diagnoses, procedures, illnesses, and surgery you or your
family had. Hospitals keep these records electronically. However
different hospitals may not have access to these records. Personal
medical data may be managed on blockchain. Each individual will have
access to their own record. The identity of individual will be kept on
their mobile phone and will be readable via a barcode. The blockchain
may either store a full copy of the individual's health records. In this
case data storage requirement could be high. Another option is to limit
the data kept on the blockchain to only records of individuals' hospital
visits, while having respective hospitals manage details of their
patients' health records. In both cases usage of blockchain has the
potential to cope with healthcare information interoperability
challenges.

> 

**Transparency in the supply chain in Agriculture**
---------------------------------------------------

A farmer produces vegetables. Before the product reaches to the
end-customer, it goes through a chain of intermediaries. Each
intermediaries puts their own price on the product. And the price
between the farmer and the end-customer is steep. During this process,
conditions such as temperature and humidity values of the products are
also not transparent to all the parties involved. Can blockchain help
this process to be more transparent? For example, in a pilot project,
Walmart, one of world's largest food chains, was able to track a product
from a farm all the way to its store shelves. The company expects that
the tracking process, which historically has taken days or weeks, could
be cut to minutes or even seconds.

We can implement a blockchain-based IoT solution to track physical
products and verify attributes from origin to point of sale to provide
supply chain transparency and traceability.

![](media/image16.png)

> Figure 5 - Blockchain based IoT solution (PWC, 2018)

The figure above explains a blockchain based solution. It was presented
by PWC for Indian agriculture sector. We strongly believe similar
problems exists in Turkish agricultural sectors, thus it could be
applicable in Turkey too. They explain the system as below:

• A farmer takes a geo-tagged image of his/her farm during harvest. The
harvest is packed into gunny bags (or any other storage means) where the
farmer takes a geo-tagged image of the packing area. The farmer may also
share data pertaining to financing or benefit schemes using a mobile
phone. The farmer then takes the gunny bags to the nearest buying agent.

• The buying agent then registers the produce of the farmer. The agent
verifies and registers the produce, along with the following
information:

\-- Details of the farmer

\-- Quantity procured

\-- Other details of the produce

\-- Geo-tagged image of the farm

• Once the produce is registered, a QR code is generated automatically.
The buying agent prints the QR code and sticks it on the gunny bags.

• The buying agent then collates multiple registered produces and
creates a consignment. Each consignment box is secured with a magnetic
reed switch which generates an alarm upon being tampered with. The
consignment box is secured with a thermocouple and polymeric sensor and
a passive RFID tag.

• The weight of the consignment is checked before it is shipped. This
weight is then fed into the blockchain by the buying agent. The
consignment gets a QR code, which is immutably linked to the QR codes of
the bags in the consignment. A smart contract is initiated for the
consignment.

• During transportation, the sensors track the storage conditions of the
consignment. The passive RFID tag enters a time stamp at the start of
the journey and a time stamp at the end of the journey at the
warehouse/processing plant.

• Any violation of the expected time taken, storage conditions or
tampering will be dealt with as a violation of a smart contract on the
blockchain. For example, if frozen fruits are being transported and the
temperature of the consignment is expected to be below zero degree
Celsius at all times, a violation shall be recorded by the smart
contract if at any point during the journey the temperature touches zero
degree Celsius.

• Similar parameters are also captured at the warehouse before the
consignment is shipped to the processing plant.

• The consignment is delivered to the processing plant. The weight of
the consignment is checked and recorded in the blockchain and verified
against its original weight. A smart contract is executed. If the weight
of the consignment is not equal to the weight of the consignment
recorded by the buying agent, the consignment is rejected.

• If no violations were raised by the smart contract and the weight
matches, the consignment is accepted.

• At the primary/secondary processing plant, an employee will be able to
read the QR code of each gunny bag to trace the produce to the
geo-tagged farm (PWC, 2018).

**Other possible implementations**
----------------------------------

-   Extends IDaaS use case explained above to provide additional
    > credentials to Turkey's citizen-government portal (E-devlet) for
    > secure identity verification based on blockchain. Currently
    > E-devlet lets you use e-signature through Turkcell and Turk
    > Telekom to make use of identity incentive applications online.
    > However the e-signature process is costly and it takes time. With
    > blockchain it is more secure and cost effective. 
    
-   Create a system for assist finding missing people (like missing
    > kids.) The first 72 hours is vital to find a missing person.
    > Therefore we need a fast and efficient system. We can implement a
    > system based on Hashgraph technology. Hashgraph is a distributed
    > ledger technology using Directed Acyclic Graph (DAG) and uses
    > "gossip about gossip" with a voting algorithm. It is scalable and
    > fast. Individuals can use a mobile app to report a missing person,
    > or what they have witnessed. Individuals will share their report
    > with their contacts. The whole system will be available to the
    > police department. The police will be able to inspect frequent
    > reports.

-   Consensus algorithms are hot topics in Blockchain. Miners spend a
    > lot of energy. In forums like Stack overflow a lot of questions
    > are being asked. Much of them are programming problems and they
    > can be reducted to mathematical problem. What if we create a new
    > consensus algorithm that takes input from a pool of real
    > programming or mathematical questions, solve them and get
    > approved. The approval rate will be determined by the number of
    > the questions and the price of each questions. People will post
    > their own question to the pool. For each question they will
    > determine how much they are willing to pay which will be the price
    > of the question. A mining group will be able to contain a set of
    > machines and / or a group of people. The problems will be solved
    > either manually by the people, or semi-automatically, or fully
    > automatic (matrix calculation etc.) This has the potential to
    > reshape freelance jobs. Imagine if artificial intelligence and
    > machine learning is so powerful that the machine understands the
    > question and responses with artificial intelligence. Mining groups
    > could be dedicated in solving problems in specific areas. For
    > examples some could be expert in dynamic programming, some in
    > greedy algorithms, or cloud computing. The idea is open to
    > suggestions. But the idea is making use of the processing power of
    > the mining machines with real world problems. Of course the miners
    > will earn coins as a reward mechanism.

-   Mobile resource sharing managed by blockchain technology, incentive
    by blockchain crypto currency. Example: your cell plan has unlimited
    data. You share it with other people. Other people connect to the
    internet by using your mobile device as a hub or proxy. They pay you
    in cryptocurrency. Or you share some files and folders through your
    mobile device.

-   Digital property rights management and access management with
    
-   Create a charity donations tracking system. Assuring the funds being
    > requested are legitimate foundations and donors know that their
    > donations are going toward the cause they want.

-   In the area of blood donoring, keep the movement of the donored
    > blood in Blockchain. In this way the donors will know where
    > exactly their blood is going, assure them that the blood is
    > reaching to those in need. Such a system can be applied to Turkish
    > Kizilay.

-   Create a blockchain based parking system. In big cities it is very
    > painful to find a parking lot. Connect all the parking services
    > and lots via IoT devices with a shared blockchain ledger. Automate
    > the payment via crypto currency. Navigate the drivers to the first
    > available parking lot. The system will decrease the traffic. And
    > it will create a lot of data for better utilization of artificial
    > intelligence and machine learning algorithms.

-   Create a blockchain based mobile service share (data, talk, and sms)
    > between mobile operators. For instance let's say you are on
    > Vodafone. You travel to somewhere which Vodafone signal is low,
    > thus accessing the internet using Vodafone is slow. However
    > Turkcell signal is better. Make an automatic process to pick
    > Turkcell over Vodafone. You will still be charged by Vodafone with
    > a partially higher cost. The Blockchain service will enable
    > communication between Vodafone and Turkcell for the cost, billing,
    > service, availability, etc. For Information Service Providers,
    > implementation of smart contracts in roaming and other cases
    > allows for near-instantaneous charging, thus leading to improved
    > revenue assurance and fraud reduction.

References
==========

> Alexandre, A. (2018). *Huawei Releases Bitcoin Wallet In App Store,
> Pre-Installed On All New Smartphones*. Retrieved from
> cointelegraph.com:
> https://cointelegraph.com/news/huawei-releases-bitcoin-wallet-in-app-store-pre-installed-on-all-new-smartphones
>
> Coininsider. (2016). *Blockchain for intellectual property
> management*. Retrieved from
> https://www.coininsider.com/huawei-blockchain-digital-property-rights-management/
>
> Davenport, C. (2018). *Huawei in talks with Sirin Labs to develop
> \'blockchain-ready\'* . Retrieved from androidpolice.com:
> https://www.androidpolice.com/2018/03/24/huawei-talks-sirin-labs-develop-blockchain-ready-phone/
>
> Deloitte. (2018). *Blockchain @ Telco How blockchain can impact the
> telecommunications industry and its relevance to the C-Suite.*
>
> Diender, E. (2017). *Blockchain in smart cities*. Retrieved from
> http://3ms.huawei.com: http://3ms.huawei.com/km/blogs/details/5207619
>
> Followmyvote. (2018). *followmyvote*. Retrieved from
> https://followmyvote.com/
>
> Forum, W. E. (2015). *Technology Tipping Points.*
>
> Huawei. (2017). *Huawei BlockChain White Paper.*
>
> Huawei IT Solution Forum. (2018). *Blockchain Training*. Retrieved
> from 3ms.huawei.com:
> http://3ms.huawei.com/hi/group/1008137/thread\_6973229.html?mapId=8670829
>
> Huawei Middle East, M. S. (2018). *Blockchain - A Huawei Middle East
> perspective on the technology, its presented opportunities, and
> challenges.*
>
> Hyperledger. (2018). *Hyperledger Fabric*. Retrieved from Hyperledger
> Fabric: https://www.hyperledger.org/projects/fabric
>
> Hyperledger Caliper. (2018). *hyperledger/caliper*. Retrieved from
> github.com: https://github.com/hyperledger/caliper
>
> Institute, N. R. (2016). *Survey on Blockchain Technologies and
> Related Services FY2015 Report.*
>
> Lomas, N. (. (2015). *Everledger is using blockchain to combat fraud,
> starting with diamonds*. Retrieved from
> https://techcrunch.com/2015/06/29/everledger
>
> R. N.-P. (2017). The nuts and bolts of blockchain technology.
>
> Martin Valenta, P. S. (2017). *Comparison of Ethereum, Hyperledger
> Fabric and Corda*. Retrieved from medium.com:
> https://medium.com/\@philippsandner/comparison-of-ethereum-hyperledger-fabric-and-corda-21c1bb9442f6
>
> Nakamoto, S. (2009). Bitcoin: A peer-to-peer electronic cash system.
>
> PWC. (2018). *Blockchain: The next innovation to make our cities
> smarter.*
>
> R3. (2018). *r3.com*. Retrieved from r3: https://www.r3.com/
>
> *What Is a Digital Signature?* (2018). Retrieved from instantssl:
> https://www.instantssl.com/https-tutorials/digital-signature.html
>
> Zhao, W. (2018). *Huawei Seeks Patent for Blockchain Rights
> Management*. Retrieved from CoinDesk:
> https://www.coindesk.com/huawei-seeks-blockchain-patent-to-protect-intellectual-property-rights
