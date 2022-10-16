A Blockchain-based Decentralized Cloud Storage with“Keeper-and-Distributor” Systems:
====================================================================================

How a Decentralized Cloud Storage System Can Solve Today’s Cybersecurity Problems.
----------------------------------------------------------------------------------

> Disclaimer: “This article is a final deliverable from Prof. Luyao Zhang’s project entitled “Trust Mechanism Design: Blockchain for Social Good,” supported by the 2022 Summer Research Scholarship (SRS) program at Duke Kunshan University. We give many thanks to DKU 2022 SRS program and the SciEcon Insight editorial board.”

Figure 1: Article Flowchart

**Introduction**
================

The utilization of the cloud to deliver digital services to end users has increased in popularity in the last decade as more businesses switch from storing and building their systems on local offline-based backend to one that is stored in the cloud. This trend is observed in the way we store data, as it has shifted from that storing data into physical hard drives, to upload data into a “digital” hard drive — the term where “cloud storage” was coined from.

Majority of today’s cloud storage services are owned and hosted by major tech companies, including, and most notably, Amazon web services (AWS), whose infrastructure supports the three types of cloud storage systems, namely: (1) object-based storages, (2) file-based storages, and (3) block storages, each of which can be used appropriately to one’s needs. However, these cloud storages are, most of the time, stored and governed by a centralized authority, such as Amazon.

Centralization gives rise to the two main problems that are discussed extensively in this paper. First of which are vulnerability and cybersecurity-related issues ranging from data breaches to ransomware deployment. Second is the issue of data privacy and obscurity– users of cloud storage have no knowledge of where their data is routed to and who has access (besides them) to it.

The goal of this paper is to propose an alternative cloud storage system that has the following features: (1) a decentralized authority that manages/hosts the cloud storage, (2) infrastructure that is built on a blockchain, and (3) a “keeper-and-distributor” system. This proposed cloud storage system is worthwhile to research and implement because it solves all the problems I’ve stated above. I’ve outlined this paper to include a background to cloud computing, an in-depth discussion of the features of this proposed system, and a comparative case study.

Figure 2: Table Showcasing Top 2 Cybersecurity Issues Addressed in This Paper

**Background**
==============

**Types of cloud storage:** There are currently three types of cloud storage: (1) object-based storage, (2) file-based storage, and (3) block storage.

[Figure 3: Types of Cloud Storages](https://nfinit.com/types-of-cloud-storage/)

In [Object-based storage](https://www.redhat.com/en/topics/data-storage/what-is-cloud-storage), data is treated as objects and involves a process where it is broken into pieces and spread out among hardware.

[Figure 4: illustration of object-based storages](https://en.wikipedia.org/wiki/File:High_level_object_storage_architecture.svg)

This data has an identifier and metadata. The identifier allows the object to be found in a system and the metadata contains the object’s detailed information. This type of storage system is most suitable for storing objects like videos and photos on Facebook and Weibo, songs on Spotify or QQ music, or files stored in “Infrastructure-as-a-Service” (IaaS) cloud storage systems like Dropbox [(Chandrasekhan et.al, 2014)](https://www.gartner.com/en/documents/2664817) and Mega; this is because the objects are highly available and highly durable. A drawback, however, is that objects themselves are not flexible to editing, which means that you cannot change object information, only create entirely new ones ([Redhat, 2018](https://www.redhat.com/en/topics/data-storage/what-is-cloud-storage)).

File storage systems on the other hand treat data as files stored in folders and can be located using paths; they have a limited amount of metadata enough for the computer to search for the file. A good example of this would be the default file manager for windows.

[Figure 5: illustration of file-based storages](https://www.redhat.com/en/topics/data-storage/what-is-cloud-storage)

File storage systems are most useful when downloading single and small files, such as word documents or pdf files, since these are easier to navigate. The disadvantage is that file-based storage systems must scale out by adding more systems, rather than scale up by adding more capacity([Redhat, 2018](https://www.redhat.com/en/topics/data-storage/what-is-cloud-storage)). Each system offers its unique advantages. On the one hand, a file storage system is apt for navigation and storage at an offline and local level, whereas object-based storage is recommended for storing data online in the cloud.

Block-based storage systems divide data into evenly sized and smaller blocks of data, each with its own address but with no metadata. The unique characteristic of block storage is that users can configure or partition each block to adjust to the operating system accessing the block of data.

[Figure 6: Illustration of block-based storage](https://www.redhat.com/en/topics/data-storage/what-is-cloud-storage)

Structured database storage, random read/write loads, and virtual machine file system (VMFS) volumes are exemplary examples. It also scales infinitely as the more data until the petabyte, which means that block storages are best for handling enterprise-sized data ([Porter et.al, 2014](https://www.druva.com/blog/object-storage-versus-block-storage-understanding-technology-differences/)).

**SaaS vs. PaaS vs. IaaS**

In order to build infrastructure in the cloud, it is important to be able to distinguish between these three types of cloud computing:

[Figure 7: Illustration of the coverages of SaaS, PaaS, and IaaS](https://101blockchains.com/blockchain-iaas-vs-paas-vs-saas/)

**Infrastructure as a Service (IaaS):** IaaS is scalable and provides a pay-as-you-go service. It communicates directly with the end user, with an already-developed web interface or dashboard that users can simply navigate through ([Bigcommerce, n.d.](https://www.bigcommerce.com/articles/ecommerce/saas-vs-paas-vs-iaas/)). Users can build applications on the interface provided to them without the need to have their own data centers for storage, since servers, networking, virtualization, and storage are all provided by the IaaS provider. Prime examples of an IaaS solution are [Cisco meta cloud](https://www.cisco.com/c/en/us/solutions/cloud/index.html) and Google Compute Engine (GCE), which lets you run virtual machines based on [Google’s](https://cloud.google.com/compute) backend infrastructure.

In IaaS, only four components are provided to you: storage, networking, data centers, and servers. As a user you are in charge of managing the server, scaling the server, and writing your own code in your own runtime environment.

**Platform as a Service (PaaS)/ Backend as a Service (BaaS):** While in IaaS, the software is already pre-packaged for the end-user, in PaaS and BaaS platforms, the users become developers, easily creating their own software, running, and managing their own applications using the coding environment and tools provided by the platform ([Iredale & Gwyneth, 2021](https://101blockchains.com/blockchain-iaas-vs-paas-vs-saas/)).

In BaaS, PaaS, while users obtain the same four benefits of IaaS, an additional benefit of PaaS/BaaS is that the provider will manage the server (middleware/OS) for you, and give you a runtime environment to deploy code. You develop the applications and handle your own data.

**Software as a Service (SaaS):** In SaaS, the features stated above are provided including the application; user data is submitted to the platform as well. SaaS is not intended for developers who are looking to develop their own applications, since most SaaS users rent all the infrastructure, middleware, and software, and the user data is sent to the SaaS platform provider. The service provider “will ensure the availability and the security of the app and your data as well” ([Microsoft, n.d.](https://azure.microsoft.com/en-us/overview/what-is-saas/)).

**Proposal**
============

The main features of my proposed decentralized cloud storage system are:

1.  A keeper-and-distributor system
2.  Blockchain-based SaaS/BaaS/PaaS/IaaS systems
3.  Cloud governance using smart contracts
4.  Data audit trail stored in blockchain
5.  Block-based and object-based storage
6.  Seed phrase to improve storage access and security

**Keeper-and-Distributor Framework:**

I derived my initial idea of a keeper-and-distributor framework from the way data is handled in Block-based storage systems. The process follows that after the uploads a block of data into the decentralized storage system, the system (1) divides the data into several smaller chunks of data, and encrypts them, turning them into encrypted data fragments. (2) the second process involves sending encrypted data fragments into a distributor system. (3) The “distributor” system then sends these encrypted data fragments into “keeper” systems. The function of keeper systems is to store these data fragments in data centers. “Keepers” are paid annually by the cloud storage system to store people’s data: think of it as paying rent to store virtual data into another individual’s data center, but instead of paying rent to a centralized company, such as Dropbox or AWS, you are paying the data center directly to store your data. Figure 5 illustrates the six-step process:

Figure 8: illustration of the keeper-and-distributor framework in a decentralized cloud storage system

**Blockchain-based SaaS/BaaS/PaaS/IaaS systems and Other Features:**

This paper utilizes three blockchain applications. The first application is building the keeper-and-distributor system on the newest internet blockchain, the [Internet computer](https://internetcomputer.org/). It is a lot easier for web2 internet apps to communicate with software built on an internet-based blockchain.

The second application is the implementation of smart contracts to create data audit trails. The purpose of this smart contract is to read, write, modify, and delete data on the internet blockchain. Instead of writing new crypto transactions, it will be writing data audit transactions, such as which keeper data centers the encrypted data fragments are sent to, and so forth This is to ensure that users have full ownership and knowledge of where their data is routed to.

The third application of blockchain is found in the manner in which this cloud storage system will be provided to its customers. It can be provided in the form of a SaaS  solution  where users interact with the decentralized cloud software, upload their files, and provide them with a dashboard, storage, networking, middleware, and other tech-blockchain solutions. It can also be provided in a **BaaS/PaaS** manner, where users will have the ability to develop their own applications on the same internet computer blockchain; this way, developers can create their own cloud computing software that can communicate with the decentralized cloud software.

The two types of cloud storage offered are block-based storage systems, which are best suited for large corporations, and object-based storage systems for regular users.

For storage access and user credentials, seed phrases can be utilized to enhance account security — the same technology that encrypts cryptocurrency wallets.

**Case Study**
==============

**Security Risks in Today’s Cloud Storage Systems**

[Figure 9: Rightscale 2018 State of the Cloud Report](https://news.lenovo.com/wp-content/uploads/2018/09/RightScale-2018-State-of-the-Cloud-Report.pdf)

[The RightScale 2018 State of the Cloud report](https://news.lenovo.com/wp-content/uploads/2018/09/RightScale-2018-State-of-the-Cloud-Report.pdf) has identified that the top challenge/risk in cloud technology is maintaining a secure cloud. There have been multiple incidents of cloud hacks and data breaches over the past decade, which evidences that **maintaining security in centralized and closed-source software is almost impossible and is resource-costly.**

A more up-to-date study by the [Thales Global Cloud Security Study in 2021](https://cpl.thalesgroup.com/cloud-security-research) reports that: “40% of organizations have experienced a cloud-based data breach in the past 12 months. Despite these incidents, the vast majority (83%) of businesses still fail to encrypt half of the sensitive data they store in the cloud.”

The reason these data breaches are so prominent is due to the lack of compartmentalization, which is a feature always present in cloud storage hosted by centralized entities. Not to mention that these companies have insiders that aid in data breaches, some of the most notable include:

1.  **SolarWinds hack:** which resulted in the leakage of almost 33,000 customers that use their Orion software. A malicious code was inserted into an Orion update, targeting over 18,000 customers after installing the infected update. The victims are not simply day-to-day users, but rather large companies, “high-profile clients, including Fortune 500 companies and multiple agencies in the US government. ([Jibilian & Canales, 2021](https://www.businessinsider.com/solarwinds-hack-explained-government-agencies-cyber-security-2020-12)).

**Hacking method:** supply chain attack through insertion of malicious code.

1.  [**Dropbox 2012 data breach**](https://www.techrepublic.com/article/2012-dropbox-hack-worse-than-realized-68m-passwords-leaked/)**:** over 68m users’ email addresses and passwords was leaked to the internet after Dropbox’s database was hacked.

[**Hacking method**](https://www.techrepublic.com/article/2012-dropbox-hack-worse-than-realized-68m-passwords-leaked/)**:** user credentials from other data breaches were used to hack the database and access user accounts.

These two major data breaches provide the argument that centralized systems without compartmentalization cannot provide grounds for good cybersecurity. Even if your own system is not compromised, data breaches from other systems can be used to access your own system. In the case of Dropbox, it was not their own framework that was hacked, but rather information from another data breach was used to log into their databases, where malicious code was deployed. Solarwinds, on the other hand, had a compromised sector in their digital supply chain, enabling it to affect all the other subsystems.

**How a decentralized cloud storage system prevents this:**
===========================================================

My proposal uses compartmentalization as a means to prevent malicious code from affecting all the other subsystems once a sector of the database is compromised. Other types of hacks, especially a supply chain type of hack, prevent the whole infrastructure from being infected because our data centers are decentralized; the data stored in these centers are also encrypted fragments, inaccessible if not combined with other encrypted fragments stored in other data centers. Should a data center get compromised, hackers will need to gain access to other data centers in order to access the data. For hacks such as account and user credential hacks, similar to the 2012 Dropbox data breach, the implementation of seed phrases as a security feature are sufficient to prevent these from taking place.

**The Keeper-and-Distributor Framework and Content Delivery Networks (CDNs)**
=============================================================================

In more traditional and non-blockchain-based frameworks, online services are delivered faster and more efficiently to the end user because of a technology we call “nodes”. A network of distributed nodes is called a Content Delivery Network (CDN) and these CDNs are able to deliver contents faster because it has nodes that are deployed in multiple locations, and also it has the ability to “cache” contents, which makes page loading faster and reduces latency ([CDNetworks, 2021](https://www.cdnetworks.com/web-performance-blog/how-content-delivery-networks-work/))

[Figure 10: Content Delivery Network Illustration](https://www.plesk.com/blog/tag/content-delivery-network/)

My idea of having multiple keeper and distributor centers was initially inspired by the technology involved in CDNs — having multiple nodes/proxy servers would mean less latency and faster services in the same way that having multiple keeper and distributor systems, similar to nodes, would enable faster cloud storage access. However, there were a lot of issues involved in cache-operated systems. First, it was quite vulnerable to DOS (denial of service) attacks, in fact, a new hacking method called CPDoS (Cache Poisoned Denial of Service) was recently coined to describe this new class of web cache poisoning type of attack ([CPDoS, n.d](https://cpdos.org/)). Secondly, having multiple nodes or proxy servers that are connected to one central server opens up vulnerabilities to the supply chain type of attack. It is very difficult for the central server to maintain and protect all of its CDN nodes and servers. While currently, the go-to method for ensuring the protection of CDN nodes is through “hash validation” and through third-party audit companies, the main security flaw is still there — it’s the fact that there is still this possibility of a malicious node compromising other nodes and eventually the entire system; there is also an issue of expansion — the more you increase CDN landscape and the number of nodes you have, the more you increase the attack surface ([ProcessBolt, n.d.](https://processbolt.com/supply-chain-attacks)) This is the issue of centralization, as I have discussed extensively.

A keeper-and-distributor system is different from CDNs in the sense that they are first, not cache-based systems. Second, KADs are decentralized, with each node/data center being connected only to the distributor and not other keepers. Lastly, whatever data is stored in KADs is encrypted and inaccessible without the two other data fragments stored in the two other data centers.

We can briefly establish a threat model: once a keeper node gets compromised, we can immediately lock the distributor center assigned to that node. Since keeper nodes only have connections to distributors, locking the distributor center immediately will prevent other nodes from being compromised.

**Roadmap of Implementations**
==============================

Figure 11: Roadmap for Implementations

**Final Notes and Potentials**
==============================

While decentralization and building web3 applications are still at its birth, there is a lot of potential for this technology to be successful, since users will certainly be willing to invest in a cloud storage system that is both secure and privacy-respecting. The majority of big tech corporations sell user data to third parties for profit, for targeted advertising, and even have agreements with governments to access user data without consent. With decentralization, blockchain technology, and open-source technology, the majority of users can take control of their data and work collectively to enjoy enhanced security.

There are many potentials for implementing this on a blockchain. Web3 applications built on the same Motoko blockchain can communicate with the decentralized cloud storage in order to create a web3 ecosystem. A good example would be in eCommerce and business analytics as web2 stores need storage systems to store data. Our block-based storage system can scale infinitely and support a larger number of stores at an enterprise level. We can also import this storage system to other blockchains, especially to Ethereum or Solano blockchain where the majority of web3 apps are built today.

About the Author
================

Josh Manto is a junior majoring in Data Science at Duke Kunshan University (DKU). Originally from the Philippines, he received a scholarship prior to joining the university for academic merit. He has a solid foundation in Data Science, a rich experience in research, and has since managed two e-commerce startups to this day.

His areas of interest include big data, machine learning, and blockchain applications, specifically in cloud computing and mechanism design. He is currently working under Professor Luyao Zhang as a research and lab leader for her Blockchain+ Research Program.

See his [**LinkedIn**](https://www.linkedin.com/in/josh-manto/)

Acknowledgments:
================

**Associate Editor:** Xinyu Tian

**Chief Editor:** Prof. Luyao Zhang
