**On the Mechanics of Blockchain Security**
===========================================

An AMA Interview for Prof. Fan Zhang about how recent advances in privacy and security technology empowers DeFi Applications on blockchain
------------------------------------------------------------------------------------------------------------------------------------------

**About Prof. Fan Zhang**
=========================

**Introduction to Prof. Fan Zhang:**

![](https://miro.medium.com/max/1400/0*lu1rnK2SRAFv8oBW)<br />Figure  1: Prof. Fan Zhang

Dr. Zhang is an Assistant Professor in the Department of Computer Science at Duke University. His recent research interests include the security, privacy, and scalability of decentralized systems, in particular those enabled by blockchains and trusted execution environments (TEEs). His works have been featured in Forbes, MIT Tech Review, IEEE Spectrum, CoinDesk, BitcoinMagazine, and numerous other blockchain news outlets. Several of his works have seen industry uptake. He received Ph.D. in Computer Science from Cornell University, advised by Prof. Ari Juels. He is a member of IC3 and a recipient of an IBM Ph.D. Fellowship for 2018–2020. He received B.Eng from Tsinghua University, China. In his separate capacity, he does research at Chainlink Labs.

Watch our AMA interview for Prof. Fan Zhang on our [YouTube channel](https://youtu.be/EqIagNge018), SciEcon.

Read the Interview Scripts with annotations and citations.

**Question 1**
==============

**Xinyu Tian:**

> Professor Fan Zhang, we read your article about the [_DECO, a privacy-preserving oracle protocol, and CanDID_](https://www.deco.works/)**,** a  platform for realizations of decentralized identities. We realize that **communication security** and **internet identity security** are currently hot topics in cryptography and distributed networks. Your research results will significantly impact the future direction of network security technologies. So, we appreciate your participation in your AMA interview session.

**Zesen Zhuang:**

> We believe that your pioneering work will benefit the development of blockchain and fintech and inspire scholars researching this field. Let’s get into our interview. Here is the first question. In your conference article**,** [_DECO, a privacy-preserving oracle protocol, and CanDID_](https://www.deco.works/), you mentioned that some financial applications based on smart contracts would be difficult to implement without DECO. So how do you think blockchain and fintech like DECO will reshape how scholars do finance research and collaborate with practitioners?

**Prof. Fan Zhang:**

> DECO essentially gives the ability to let smart contracts consume private data. For example, at DeFi \[1\] applications and particularly DeFi-based loans, if you want to take out a $100 loan, you need to put down a $200 collateral. This [_over-collateralization_](https://www.investopedia.com/terms/o/overcollateralization.asp) is economically inefficient.

![](https://miro.medium.com/max/1400/0*yG8rMqyavbu0c82i)<br />Figure  2: [Crypto Loans](https://www.yield.app/post/defi-lending-and-borrowing-guide)

> The inefficiency comes from the difficulties of accessing credit history while protecting privacy. DECO overcomes the challenges by providing a privacy-preserving way to utilize financial records for risk assessments. [_Chainlink_](https://chain.link/)  has licensed DECO. Our team is working on further developing DECO integrated DeFi Applications. Our work will revolutionize how people transact in DeFi. In my understanding, one of the fascinating things about working in this space is that industry and academia collaborate a lot. Professors are working with pioneers in the industry, and practitioners also care about academic research, which is rare in other disciplines.

**Prof. Luyao Zhang:**

> Sounds very interesting! In Economics, professors start to collaborate more with practitioners in the area of Fintech. I’m impressed to learn from you the exciting story: From the very start, computer scientists have a natural collaboration between academia and industry on the blockchain. That’s very special!

**Prof. Fan Zhang:**

> I think it’s a scarce opportunity for researchers. I can name many startups founded by researchers and many firms that have licensed technology from universities. I feel particularly excited about how fast adoption can happen in the blockchain world. It’s amazing.

Question 2
==========

**Xinyu Tian:**

> Thank you so much for sharing your ideas behind the DECO protocol and its potential application in the blockchain. It is exhilarating to hear about the rapid development of blockchain technology and the interdisciplinary research it stimulates. Here comes our second question: in your conference paper [_CanDID: Can-Do Decentralized Identity with Legacy Compatibility, Sybil-Resistance, and Accountability_](https://urldefense.com/v3/__https://doi.ieeecomputersociety.org/10.1109/SP40001.2021.00038__;!!OToaGQ!6Enw8eVMtlrOnh4htQwCQWmIUM0zfiKQIZ2Knb1d2fTrA30PxgbQ-QFZkrxZC3Py$), you introduced the idea of empowering end-users with the management of their credentials, and you described CanDID as a platform for decentralized identity. What do you think about the current situation in cybersecurity in blockchain and decentralized systems?

**Prof. Fan Zhang:**

> Just to clarify, I didn’t invent those visions. **Decentralized identity** or self-sovereign identity \[2\] was an existing idea that kind of goes back to the early days of the Internet. Let’s relate to your question: why does it happen now?

![](https://miro.medium.com/max/1400/0*99us0gcMgeoe38tV)<br />Figure  3: [Decentralized Identity](https://anarsolutions.com/decentralized-identity/)

> The revolution comes from the emergence of new security and privacy technologies. The key technology that enables CanDID is **blockchain technology**, which has improved in recent years and **advances in cryptography**, among those especially believed to be impractical, such as multiparty computation \[3\], zero-knowledge proofs \[4\]. Those are expensive and powerful cryptographic tools. Until very recently, if you ask people about examples of MPC **(**multiparty computation**),** they will tell you that two millionaires want to compare who is more wealthy and don’t want to reveal their net wealth to each other. People have been working on such abstract examples for years because large-scale deployment was not there yet.
> 
> However, we have seen many advancements in this field in recent years, and CanDID benefits from those. With the powerful tools becoming more practical, we can build advanced systems such as CanDID and many more. The Great advancement in recent years in security and privacy technology enables all of this.

Question 3
==========

**Zesen Zhuang:**

> Thank you for sharing your ideas in the cybersecurity aspect, which is also the issue that Dfinity is facing in its [_Internet Identity_](https://dfinity.org/faq/internet-identity) service. The last question of this interview is about the internet computer itself. The Internet Computer is the first frictionless blockchain with web speed and internet-scale throughout the world. It extends the functionality of the public Internet so that it can host backend software, transforming it into a global computing platform. Do you think IC, or any other decentralized technology, can solve the Blockchain trilemma (decentralization, scalability, security)? How do you think the IC can empower the financial industry?

**Prof. Fan Zhang:**

> I try not to discuss fluffy stuff like trilemmas because Blockchain solves the trilemma by making certain compromises. I don’t know Dfinity well enough to comment specifically, but I don’t think there’s fundamentally an exception. I think the discussion of this type has to be more precise and more concrete. It’s exciting to see new platforms like what Dfinity is launching and driving the development in that direction.

Discussion
==========

**Prof. Luyao Zhang:**

> I’m curious about your insights on the security part of the blockchain trilemma because you’re an expert on it. For example, for the  front-running \[5\] that we have discussed, it has been a historical problem in finance for years caused by intermediaries. Blockchain claims to cut intermediaries in financial transactions. I was astonished to know the front-running problem has again become a problem for the transactions on the blockchain. Is there any intuitive way that we could finally solve the front-running problem? I’m not sure whether the Internet Computer is going to solve it. It seems they are using a new consensus algorithm, but how can we solve the front-running problem intuitively?

![](https://miro.medium.com/max/1362/0*_r0Sd9eQD6Rvd_Ll)<br />Figure  4: [Front Running](https://www.wallstreetmojo.com/front-running/)

**Prof. Fan Zhang:**

> That’s an excellent question. Recently there have been heated discussions between practitioners and academia. The answer to your question depends on who you ask. There are generally two directions: Some believe front-running can be solved or minimized by building platforms with built-in “fairness” guarantees. First of all, we have front-running in the blockchain because you can think about the blockchain as a temporary centralized system. At a given time, only one miner is dictating the ordering of transactions. Some people believe that we can reduce front-running to a low level by building a “fair” consensus protocol.  
> On the other hand, others claim that MEV is kind of fundamental. You can build new protocols, but new protocols will have unique problems and new front-running opportunities. Because fundamentally, whenever there is information asymmetry and temporary centralization, you will have parties with more power than others, which will lead to MEV. An entirely egalitarian system seems very hard to build, and some people believe that we can’t solve the problem of front-running. In their views, we can democratize the opportunity for front-running attacks or extract MEV.

**Prof. Luyao Zhang:**

> It sounds like an unsolvable question, and it’s promising for us to work on it.

**Prof. Fan Zhang:**

> I think it requires input from more than just computer science, and even defining the meaning of fairness is non-trivial, and we could write an entire paper just on that. Compared with the computer science point of view, the definition of fairness in finance and the economy is even more complex, especially if you want to realize it in a real-world system.

**Prof. Luyao Zhang:**

> Yes, economists often disagree as well, and it would be a lot to say. I have one curious question as a user of the blockchain. The identity issue often puzzles us. Right now, we need to have physical tools like [_Yubikey_](https://www.yubico.com/)  for the computer or the blockchain to understand our identity.

![](https://miro.medium.com/max/1400/0*vuQB38dW69u2oP80)<br />Figure  5: [Yubikey](https://zapier.com/blog/what-is-a-yubikey/)

> So, we would worry that if we lost the key, we would lose everything. Then, maybe we don’t have enough options to trust that our money on the blockchain is much safer than the current status quo. We might prefer protection from the police or the government so that when we lose the key to our bank account, we can have our ID reset. However, on the blockchain, we have to be our custodians. How do you feel about that?

**Prof. Fan Zhang:**

> You’re saying we’re in trouble if we advertise self-custody of identity by securing a key, and we lose that key. We thought hard about this issue in the CanDID paper, and one of the goals is to solve this key management challenge in a usable way. Key management has been a decade-old problem since the birth of public-key cryptography. The problem is not new, but in the blockchain setting, the consequence is a lot more severe in that if you lose your key — you could lose a lot of money or even your identity. We had some ideas in that paper. For example, there are ways to build a key storage system where you can retrieve your keys. It’s a balance between security and usability.
> 
> The most useable way is that we have a centralized third party, and we give our keys to that party, and then that party will do the job of backing up the key and so on. We ask for the keys when we need them. That’s what people essentially are doing when they store their bitcoin on [_Coinbase_](https://www.coinbase.com/). Users don’t have to manage the keys because Coinbase does so. The drawback is that you don’t really have your keys and that third party could be malicious or could lose your key to attackers and so on. Therefore, the most “secure” version might be that you do your own thing. For example, what I do, which is simple, is print out the key on paper and store it in the safe. It’s fascinating because keys are such a digital thing. But actually, one of the safest ways to keep it is to print them out and store them in the safe. In the CanDID paper, we talk about something in the middle, which is an excellent idea. It is the following: you don’t need to trust a single third party because trusting a party might bring too much risk, but what about trusting three or five parties? For example, we split the secret into three pieces, and you store them at [_Google Drive_](https://www.google.com/drive/), at [_Microsoft OneDrive_](https://onedrive.live.com/), and [_GitHub_](https://github.com/). Then, if you want to retrieve the key, you authenticate to these services using your password. People are familiar with using passwords, and it’s the same here. If you want to retrieve your key, you type your password and get back your key shares. The crucial difference is that you don’t need to trust any single party but three of them altogether. Using the secret sharing technique, we can split the key into pieces so that you need the three parts to get back your secret, and any two pieces won’t leak any information. That’s the way we propose in CanDID, and it’s not hard to implement. I think it’s an amicable solution. I want to see people adopt our CanDID solutions. However, it seems that people are still at the two extremes**.**
> 
> People who hold on to Coinbase for reasons. Coinbase has a big reputation that makes it a rational choice. However, we believe the tool for a middle-way solution is not hard to build and implement. We are curious how users will react when we make such a tool available. In conclusion, I think it’s a complex question, and there are various trade-offs.

**Prof. Luyao Zhang:**

> We want to try all the promising methods, which sounds very exciting. However, on the other hand, I found we are not at the stage yet where we don’t need police anymore. Because otherwise, malicious guys can steal your safes. Then the safes are not safe anymore.

**Prof. Fan Zhang:**

> Certainly.

**Prof. Luyao Zhang:**

> Thank you, professor Fan Zhang, and this would be the end of our AMA interview session.

**Prof. Fan Zhang:**

> Thank you for having me.

Relevant Materials
==================

\[1\] **DeFi**

Decentralized finance (commonly referred to as DeFi) is a [blockchain](https://en.wikipedia.org/wiki/Blockchain)\-based form of finance that does not rely on central financial [intermediaries](https://en.wikipedia.org/wiki/Intermediary) such as [brokerages](https://en.wikipedia.org/wiki/Brokerage), [exchanges](https://en.wikipedia.org/wiki/Exchange_(organized_market)), or [banks](https://en.wikipedia.org/wiki/Bank) to offer traditional [financial instruments](https://en.wikipedia.org/wiki/Financial_instrument), and instead utilizes [smart contracts](https://en.wikipedia.org/wiki/Smart_contract) on blockchains, the most common being [Ethereum](https://en.wikipedia.org/wiki/Ethereum).[\[1\]](https://en.wikipedia.org/wiki/Decentralized_finance#cite_note-Financial_Times_2019-12-30-1)

[Wikipedia](https://en.wikipedia.org/wiki/Decentralized_finance)

\[2\] **Self-sovereign identity**

Self-sovereign identity (SSI) is an approach to [digital identity](https://en.wikipedia.org/wiki/Digital_identity) that gives individuals control of their digital identities.[\[2\]](https://en.wikipedia.org/wiki/Self-sovereign_identity#cite_note-2)

[Wikipedia](https://en.wikipedia.org/wiki/Self-sovereign_identity)

\[3\] **Multi-party Computation**

Secure multi-party computation (also known as secure computation, multi-party computation (MPC), or privacy-preserving computation) is a subfield of [cryptography](https://en.wikipedia.org/wiki/Cryptography) with the goal of creating methods for parties to jointly compute a function over their inputs while keeping those inputs private. Unlike traditional cryptographic tasks, where cryptography assures security and integrity of communication or storage and the [adversary](https://en.wikipedia.org/wiki/Adversary_(cryptography)) is outside the system of participants (an eavesdropper on the sender and receiver), the cryptography in this model protects participants’ [privacy](https://en.wikipedia.org/wiki/Privacy) from each other.

[Wikipedia](https://en.wikipedia.org/wiki/Secure_multi-party_computation)

\[4\] **Zero-knowledge proof**

In [cryptography](https://en.wikipedia.org/wiki/Cryptography), a zero-knowledge proof or zero-knowledge protocol is a method by which one party (the prover) can prove to another party (the verifier) that they know a value x, without conveying any information apart from the fact that they know the value x. The essence of zero-knowledge proofs is that it is trivial to prove that one possesses knowledge of certain information by simply revealing it; the challenge is to prove such possession without revealing the information itself or any additional information.[\[1\]](https://en.wikipedia.org/wiki/Zero-knowledge_proof#cite_note-:0-1)

[Wikipedia](https://en.wikipedia.org/wiki/Zero-knowledge_proof)

\[5\] **Front-running**

Front-running is trading stock or any other financial asset by a broker who has inside knowledge of a future transaction that is about to affect its price substantially. A broker may also front-run based on insider knowledge that their firm is about to issue a buy or sell recommendation to clients that will almost certainly affect the price of an asset.

[Investopedia](https://www.investopedia.com/terms/f/frontrunning.asp)

\[6\] **MEV**

MEV, also referred to as _Miner Extractable Value_, is becoming a point of discussion among Ethereum developers and traders as DeFi continues to thrive on the Blockchain ecosystem.

Synonymous to a miner’s ability to decide where and when a transaction is placed on a block, Miner Extractable Value (MEV) is often used by miners to generate additional revenue on a block by reordering transactions in each block, in ways that are beneficial to them.

[medium](https://medium.com/umbrella-network/miner-extractable-value-mev-101-why-what-and-how-4bec3bc3bb2a)

Acknowledgments
===============

Interviewee: Prof. Fan Zhang

Interviewer: Prof. Luyao Zhang, Xinyu Tian, Zesen Zhuang

Advisor and Chief Editor: Prof. Luyao Zhang
