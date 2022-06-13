Recap of ETHconomics @ Devconnect 2022
======================================

Part of Computer Science Meets Economics on Ethereum Spotlight Series
---------------------------------------------------------------------

**Keywords (#hashtags):**
-------------------------

#Ethereum #Transaction Fee Mechanism #Empirical analysis #Waiting time #Consensus Security #Devconnect #Interdisciplinary #Computerscience #Economics

**Editor’s Highlights (by Prof.** [**Luyao Zhang**](http://scholars.duke.edu/person/luyao.zhang)**):**
------------------------------------------------------------------------------------------------------

*   **Research:** conduct cutting-edge interdisciplinary research that ensembles computer science and economics to converse, research, and innovate on Ethereum blockchain
*   **Innovation:** understand the effect of EIP-1559 on improving transaction fee mechanism design on Ethereum
*   **Leadership:** contribute to an open economy of the people, for the people, by the people by making code and data open-source and cultivating undergraduate research

![](https://miro.medium.com/max/1400/0*lKHh1YBuEP8NpEpb)<br />Figure  1: Feature Photo (Supported by Canvas)

> D**isclaimer**: This article is part of the Industry 4.0 Open Educational Resources (OER) Publication Initiatives jointly supported by [Duke Learning Innovation Center](https://ie.pubpub.org/) and [DKU Center for Teaching and Learning](https://ie.pubpub.org/) under the [Carrying the Innovation Forward program](https://ie.pubpub.org/). This article belongs to the OER Series №2 [Computational Economics](https://ce.pubpub.org/) Spring 2022 collection. The Spring 2022 collection is partly supported by the Social Science Divisional Chair’s Discretionary Fund to encourage faculty engagement in undergraduate research and enhance student-faculty scholarly interactions outside of the classroom. The division chair is Prof. [Keping Wu](https://scholars.duke.edu/person/keping.wu), Associate Professor of Anthropology at Duke Kunshan University. The author Tianyu Wu was the Teaching and Research Assistant for Prof. [Luyao Zhang](http://scholars.duke.edu/person/luyao.zhang) in the course: COMPSCI/ECON 206 Computational Microeconomics at Duke Kunshan University Spring 2022, when he completed the joint article.

Introduction and Deep Dive Event
================================

On Apr 21, 2022, [Prof. Fan Zhang](https://www.fanzhang.me/) and [Prof. Luyao Zhang](http://scholars.duke.edu/person/luyao.zhang) were invited by [Ethereum Foundation](https://ethereum.org/en/foundation/), a non-profit organization (NPO) that focuses on supporting Ethereum and related technologies, to give a presentation on their paper, [_Empirical Analysis of EIP-1559: Transaction Fees, Waiting Time, and Consensus Security_](https://arxiv.org/abs/2201.05574), at [ETHconomics @ Devconnect 2022](https://ef-events.notion.site/ETHconomics-Devconnect-676d73f791684e18bfae35bbc9e1fa90) in Amsterdam, Netherland.

![](https://miro.medium.com/max/618/0*XENJgyElICb8Fuy1)<br />Figure  2: [Ethereum Foundation](https://ethereum.org/static/75a7d7bf3453c8dc08adbcbce7ea2dae/2546a/ef-logo.png)

This paper was recently accepted at [ACM CCS’22](https://www.sigsac.org/ccs/CCS2022/) Conference \[1\], with the track of Blockchain and Distributed Systems, where the chair of this track is [Ittai Abraham](https://research.vmware.com/researchers/ittai-abraham), Senior Researcher at [VMware](https://research.vmware.com/). Due to the global pandemic, two distinguished scholars presented their research jointly online across time zones.

Watch the Presentation [**Documentary**](https://youtu.be/gAWcmLJxIfY) on [**SciEcon YouTube Channel**](https://www.youtube.com/channel/UCQOvF-D45s09FlajFkKzoOA)

Watch all Presentation Videos at [ETHconomics @ Devconnect 2022 YouTube Channel](https://www.youtube.com/channel/UCkGClyuefTTYZj9nU0-D71Q)

[Devconnect](https://devconnect.org/) is the first-ever featured gathering event during the week of April 18–25, 2022, focusing on different topics related to the development of Ethereum. It brings the Ethereum community together in small groups and provides a joint-built platform for in-depth cross-disciplinary cooperation and discussions, and more information can be found via their [tweets](https://twitter.com/EFDevconnect). [ETHconomics](https://ef-events.notion.site/ETHconomics-Devconnect-676d73f791684e18bfae35bbc9e1fa90) is one of the series at Devconnect, and it is a one-day session gathering researchers and developers in industry and academia looking to broaden our understanding of Ethereum economics and discussing the topics related to the economics of the Ethereum network. There are altogether 16 research presentations in this session, where topics include [layer-2 rollups](https://ethereum.org/en/developers/docs/scaling/) \[2\], [blockchain consensus](https://ethereum.org/en/developers/docs/consensus-mechanisms/) \[3\], [transaction fee mechanism](https://ethereum.org/en/developers/docs/gas/) \[4\], [cryptoeconomics](https://ethereum.org/en/learn/) \[5\], [game theory](https://www.nobelprize.org/prizes/economic-sciences/1994/press-release/#:~:text=Reinhard%20Selten%2C%20Rheinische%20Friedrich%2DWilhelms,theory%20of%20non%2Dcooperative%20games.&text=Game%20theory%20emanates%20from%20studies%20of%20games%20such%20as%20chess%20or%20poker.), etc. The main event organizer and coordinator [Barnabé Monnot](https://www.linkedin.com/in/barnabemonnot/) says in his [LinkedIn](https://www.linkedin.com/posts/barnabemonnot_ethconomics-devconnect-2022-youtube-activity-6933370356921479168-dTKQ/?utm_source=linkedin_share&utm_medium=member_desktop_web) post that:

> **Talk subjects ranged from game theory to protocol economics, theory and empirical studies, system design, modeling and simulation…** [**ETHconomics**](https://ef-events.notion.site/ETHconomics-Devconnect-676d73f791684e18bfae35bbc9e1fa90) **reflected both the interdisciplinary nature of cryptoeconomics and the excitement that comes from putting the pieces together.**

Presenters include both academic scholars and industry professionals, and they come from various backgrounds, ranging from computer science, data science, and economics, to describe how Science and Economics meet and integrate with each other on Ethereum blockchain. More information about the speakers and presentations can be found in the Appendix.

![](https://miro.medium.com/max/1400/0*vINhoWBVIM54FwyM)<br />Figure  3: [Devconnect](https://storage.googleapis.com/ethereum-hackmd/upload_83966632df3abe4e7f3b3bac6f3aabc9.jpg)

[Prof Tim Roughgarden](http://timroughgarden.org/papers/eip1559.pdf) was invited to make a keynote speech, titled as [_Mechanism Design for Ethereum and Beyond_](https://www.youtube.com/watch?v=a9SB3uXR1qw), to give an overview of the game-theoretical analysis of EIP-1559, the improved proposal of Ethereum transaction fee mechanism design, and proposed several desirable open research directions to enlighten the scholars present.

Recap of presentation
=====================

Right after Prof Tim Roughgarden’s keynote on the theoretical aspects of mechanism design for Ethereum, Prof Fan Zhang and Prof Luyao Zhang presented their interdisciplinary research on the empirical analysis of EIP-1559, which ensembles Computer Science and Economics to converse, research, and innovate on Ethereum Blockchain. The presentation slide is available via [Docsend](https://docsend.com/view/s8798vk8w3cdmjqz). You can also access their working paper online through [arXiv](https://arxiv.org/abs/2201.05574), as well as the open-access data and code through [GitHub](https://github.com/SciEcon/EIP1559). By making use of rich and valuable data from collected mempool, Ethereum blockchain, and exchanges, their work figured out three exciting major results to comply with the current theoretical results:

T**ransaction Fee: EIP-1559 has a negligible effect on the gas fee levels, however, it mitigates the intra-block difference of gas fee paid.**

With the technique of causal inference, the researchers find that with the block features: block size and block height, and exchange features: volatility and return of investment of Ether controlled, the median gas fee does not change much. This finds an echo with Roughgarden’s theoretical result that [London Fork](https://eips.ethereum.org/EIPS/eip-1559) is not a solution for scalability, that is, as the adoption rate of EIP-1559 increases, intra-block gas fee volatility decreases significantly. These results mainly imply that in the future we should further increase user experience by making fee estimation easier because people tend to be bounded rational.

![](https://miro.medium.com/max/1400/0*RgeDOXalPqI29PWe)<br />Figure  4: Transaction Fee: Visualization on Intra-block Gas Price Volatilities (Source: [Copyright@Fan Zhang and Luyao Zhang 2022](https://docsend.com/view/s8798vk8w3cdmjqz))

W**aiting Time: EIP-1559 helps to reduce the users’ waiting time and the time evaluation of opportunity cost to transact on Ethereum.**

This research group set up four Ethereum nodes across the globe to make the collection of ephemeral mempool data happen. They also created an innovative approach to deal with the issue of 50% negative waiting time in the previous research, by correcting that the calculation of the waiting time is not to use the timestamp where the transaction is included in the blockchain, but the next timestamp due to the feature of Proof-of-Work (PoW) consensus mechanism. With this correct calculation, researchers find that the average waiting time decreases from 17 seconds to 10 after London Fork, probably due to an easier fee estimation and variable size of blocks.

![](https://miro.medium.com/max/1400/0*JyjUnlZTVF9W23He)<br />Figure  5: Waiting Time: Visualization on Block Median Waiting Time (Source: [Copyright@Fan Zhang and Luyao Zhang 2022](https://docsend.com/view/s8798vk8w3cdmjqz))

C**onsensus Security: EIP-1559 does not have a huge impact on consensus security even though the block size has been increased.**

The researchers argue that EIP-1559 may negatively impact the security issue in the Ethereum blockchain, but the extent of the impact is modest. They broke the analysis of the consensus security into three dimensions: fork rate, network load, and incentives (Miner Extractable Value, simplified as MEV). They find out that the introduction of variable block size in EIP-1559 is likely to account for why the fork rate has increased by 3%, despite the London Fork, the Ethereum blockchain is still operating at a lower load than before. At the same time, as empirical data shows that MEV is becoming a larger share of the revenue from miners’ point of view, researchers conjecture that miners are being incentivized to invest more in MEV extraction.

In summary, Prof. Luyao Zhang describes how the research advances Prof. Tim Roughgarden’s theoretical research from the following three aspects:

1.  The empirical analysis of the transaction fee in this research shows that there is not much reduction on the gas fee level after London Fork, thus it serves as a counterpart of Prof Roughgarden’s theoretical work on confirming that EIP-1559 is not a solution for scalability.
2.  The empirical analysis of waiting time is actually a pure exploration and pioneer study since there is no systematic theoretical research before.
3.  The empirical analysis of consensus security in this research focuses on different aspects compared to Prof Roughgarden’s work besides the methodology differences.

![](https://miro.medium.com/max/1400/0*VRe8l6z6MnyDy0pp)<br />Figure  6: Contribution Map (Source: [Copyright@Fan Zhang and Luyao Zhang 2022](https://docsend.com/view/s8798vk8w3cdmjqz))

More about the paper
====================

This research also leaves plenty of interesting future research directions. It inspires more computer scientists and economists to collaborate on cutting-edge interdisciplinary research to solve the issues in the Ethereum blockchain through mechanism design, which comprises both profound insights and practical impacts. Notably, the research pioneers a research agenda that applies the method of [natural experiments](https://www.nobelprize.org/prizes/economic-sciences/2021/popular-information/) \[6\], the Nobel Prize 2021 in Economics which mitigates the internal validity problem in the [lab experiments](https://www.nobelprize.org/prizes/economic-sciences/2002/popular-information/) and external validity problem in the [field experiments](https://www.nobelprize.org/prizes/economic-sciences/2019/popular-information/), to conduct empirical studies of mechanism changes on Ethereum. Prof. Luyao Zhang concludes with three main advantages to explain why Ethereum blockchain data makes the empirical study with natural experiments more approachable: First, blockchain data is well recorded and transparent to free the researchers from the data availability issue; Second, all the users’ privacy is well protected in order to discord the ethics issue thanks to advanced asymmetric cryptography; Third, smart contract on the Ethereum blockchain enables an automation process to significantly reduce the data collection costs.

![](https://miro.medium.com/max/1400/0*MBPHE4Nt8Uk_nA5y)<br />Figure  7: Methodologies (Source: [Copyright@Fan Zhang and Luyao Zhang 2022](https://docsend.com/view/s8798vk8w3cdmjqz))

Second, it inspires future researchers to think about how to use a theoretical framework to rigorously describe the reason for the empirical result that the waiting time significantly decreased after London Fork. Moreover, mempool data is another important and exciting source to analyze in-depth in order to better understand blockchains in various ways. Prof. Fan Zhang also mentions in the presentation that his team is now

> **working with Ethereum Foundation under its sponsorship on a project to dig deeper into mempool data to understand blockchains in various aspects.**

Personal Reflections
====================

After watching this presentation, I am extremely inspired by how interdisciplinary collaborations can provide cutting-edge research with both profound insights and practical impacts, which is obviously not possible only by scholars from one discipline. For example, without Prof Luyao Zhang’s contribution of her expertise on the natural experiment methodology and her solid knowledge in bounded rationality and mechanism design ([Levin and Zhang 2017](https://www.aeaweb.org/articles?id=10.1257/aer.p20171030); [Levin and Zhang 2020](https://direct.mit.edu/rest/article-abstract/doi/10.1162/rest_a_00990/97700/Bridging-Level-K-to-Nash-Equilibrium?redirectedFrom=fulltext)), I couldn’t imagine how open-source data on Ethereum blockchain would ever empower causal inferences in the study of bounded rationality and mechanism design. In the meanwhile, if we did not have the mempool data collected across the globe by Prof. Fan Zhang as well as his sharp insights on the waiting time estimation corrected by a subtle but super smart trick, we would not ever be able to evaluate the effect of EIP-1559 on waiting time, one important aspect of user experience empirically. Their joint insights from economics and computer science provide us with such an intellectual feast; neither side is dispensable.

Moreover, I also admire how scholars, during the pandemic, can really turn the adversity in background, disciplines, and time zone differences into an opportunity for innovation. This innovation is indeed really hard to implement since it takes time to ensure that scholars, including two other co-authors Prof. [Yulin Liu](https://ch.linkedin.com/in/yulineth) and Prof. [Kartik Nayak](https://users.cs.duke.edu/~kartik/), whose expertise are in economics and computer science and whose primary employments are in industry and academia respectively, from different backgrounds are on the same page. The impossibility of in-person interactions and time zone differences further aggregate the difficulty. I believe it is their empathy, compassion, and intrinsic motivation in interdisciplinary research and innovation that makes it possible for us to see the new frontiers of human civilizations. As Prof. Luyao Zhang always reminds her students that the Master once said:

> **Virtue is not left to be alone; he who practices it finds neighbors.**

Last but not least, I also notice that this research team includes not only junior professors, but also some undergraduate students. I am deeply touched by the junior professors’ visions in not only pioneering seminal research at the frontier of human civilizations but also cultivating undergraduate research that would benefit generations to come. Their scholarship encourages more and more young scholars not to seek near but distant objectives and devote themselves to seminal research that could further advance the development of humanity. I am also fortunate to be one of those students accessible to research from my undergraduate years at [Duke Kunshan University](https://www.dukekunshan.edu.cn/) \[7\]. I feel such a privilege to be invited by Prof. Fan Zhang and Prof. Luyao Zhang to serve as the student project manager for their joint project entitled “Understanding the transaction fee mechanism of Ethereum blockchain,” supported by Ethereum Academic Grant 2022. How can I find a better way to spend the Summer?

Last but not least, the intellectual conversations remind me of my motto from a famous philosopher, Immanuel Kant​:

> **Ich bin von heute und ehedem, aber etwas ist in mir, das ist vor morgen und übermorgen und einstmals!**
> 
> **English Translation: I belong to today and the past, but some of my things will belong to tomorrow, the day after and the future!**

Inspired by this motto, I feel more motivated to contribute to interdisciplinary research in the future and bring a real impact to human society.

Relevant Materials
==================

\[1\] ACM CCS’22

The ACM Conference on Computer and Communications Security (CCS) is the flagship annual conference of the Special Interest Group on Security, Audit and Control (SIGSAC) of the Association for Computing Machinery (ACM). The conference brings together information security researchers, practitioners, developers, and users from all over the world to explore cutting-edge ideas and results.

[Official Website](https://www.sigsac.org/ccs/CCS2022/)

\[2\] Layer-2 rollups

Layer 2 solutions provide an approach to scale the application by handling transactions off the Ethereum Mainnet (layer 1), while taking advantage of the robust decentralized security model of the Mainnet. Rollups are designed to perform transaction execution outside layer 1 but it enables the data to be posted to layer 1 where consensus is reached. As transaction data is included in layer 1 blocks, this allows rollups to be secured by native Ethereum security.

[Ethereum — Docs](https://ethereum.org/en/developers/docs/scaling/)

\[3\] Blockchain Consensus

Consensus simply means that a general agreement has been reached. When it comes to blockchain, where the process is formalized, reaching consensus means that at least over a half (more than 50%) of the nodes on the network agree on the next global state of the network.

[Ethereum — Docs](https://ethereum.org/en/developers/docs/consensus-mechanisms/)

\[4\] Transaction Fee Mechanism (TFM)

A Transaction Fee Mechanism (TFM) is a mechanism for allocating transactions to a single block.

[Arxiv](https://arxiv.org/pdf/2106.01340)

\[5\] Cryptoeconomics

Cryptoeconomics is the applied science of building distributed systems, where properties of those systems are secured by financial incentives, and where the economic mechanisms are guaranteed by cryptography, designed to describe the practice of designing and scaling blockchains like Ethereum.

[Ethereum — Docs](https://ethereum.org/en/learn/)

\[6\] Natural Experiment

A natural experiment is an empirical investigation in which individuals are subjected to experimental and control conditions set by nature or other factors beyond the investigators’ control. The exposures are determined by a mechanism that approaches random assignment. It can significantly reduce the effect of internal validity, the extent to which a piece of evidence supports a claim about cause and effect, commonly found in lab experiments, as well as the effect of external validity, the extent to which the results of a study can be generalized to, commonly found in field experiments.

[Wikipedia](https://en.wikipedia.org/wiki/Natural_experiment)

\[7\] Duke Kunshan University (DKU)

Duke Kunshan University (DKU) is a world-class liberal arts university in Kunshan, China, that provides a variety of high-quality, creative academic programs to students from all over the world. It was founded in September 2013 as a joint venture between Duke University and Wuhan University in the United States and China.

[Website](https://www.dukekunshan.edu.cn/)

Appendix
========

Here lists all the speakers’ information in the [ETHconomics @Devconnect 2022](https://ef-events.notion.site/ETHconomics-Devconnect-676d73f791684e18bfae35bbc9e1fa90).

1\. Transaction Fee Mechanism
=============================

**Tim Roughgarden:**

Professor of Computer Science at Columbia University \[[Webpage](http://timroughgarden.org/)\]

![](https://miro.medium.com/max/900/0*fCbX6NHZPeynMVk1)

He gives a keynote speech on _Mechanism Design for Ethereum and Beyond_. The presentation video can be accessed via the [link](https://www.youtube.com/watch?v=a9SB3uXR1qw).

Contact him via [LinkedIn](https://www.linkedin.com/in/tim-roughgarden-1a594855/) or [Twitter](https://twitter.com/tim_roughgarden).

**Fan Zhang:**

Assistant Professor in Computer Science at Duke University \[[Webpage](https://www.fanzhang.me/)\]

![](https://miro.medium.com/max/1000/0*R1rHACPc2RBkVODs)

He gives a presentation on _Empirical Analysis of EIP-1559: Transaction Fees, Waiting Time, and Consensus Security_ with Prof Luyao Zhang. The presentation video can be accessed via the [link](https://youtu.be/QetFrMDBFWY).

Contact him via [LinkedIn](https://www.linkedin.com/in/fanz92) or [Twitter](https://twitter.com/0xfanzhang).

**Luyao Zhang:**

Assistant Professor in Economics at Social Science Division and Senior Research Scientist at Data Science Research Center, at Duke Kunshan University \[[Webpage](https://scholars.duke.edu/person/luyao.zhang)\]

![](https://miro.medium.com/max/1400/0*uM938sHKrovU4Q_D)

She gives a presentation on _Empirical Analysis of EIP-1559: Transaction Fees, Waiting Time, and Consensus Security_ with Prof Fan Zhang. The presentation video can be accessed via the [link](https://youtu.be/QetFrMDBFWY).

Contact her via [LinkedIn](https://www.linkedin.com/in/sunshineluyao/) or [Twitter](https://twitter.com/sunshineluyao).

**Stefanos Leonardos:**

Postdoctoral Researcher in Game Theory at Singapore University of Technology and Design \[[Webpage](https://stefanosleonardos.com/)\]

![](https://miro.medium.com/max/1400/0*kCNJ4CQZx2mYjygX)

He gives a presentation on _Dynamics of the EIP-1559 Fee Market: Predictions and Data Analytics_. The presentation video can be accessed via the [link](https://www.youtube.com/watch?v=HGZivfaZzng).

Contact him via [LinkedIn](https://www.linkedin.com/in/stefanos-leonardos/) or [Twitter](https://twitter.com/StefLeonardos).

**Ansgar Dietrichs:**

Ethereum 2.0 R&D Engineer at ConsenSys Quilt

![](https://miro.medium.com/max/1400/0*DWRskE_eKQGX-RlY)

He gives a presentation on _Notes on multidimensional EIP-1559_. The presentation video can be accessed via the [link](https://www.youtube.com/watch?v=QbR4MTgnCko).

Contact him via [LinkedIn](https://www.linkedin.com/in/adietrichs/) or [Twitter](https://twitter.com/adietrichs).

2\. Layer-2 Rollups
===================

**Ed Felten:**

Co-Founder and Chief Scientist, Offchain Labs. Retired Princeton Professor of Comp Sci & Public Affairs. Former Deputy United States CTO at White House \[[Webpage](https://www.cs.princeton.edu/~felten/)\]

![](https://miro.medium.com/max/512/0*U8XUmr5LkpySZXVb)

He gives a presentation on _Fair and sustainable fees for L2_. The presentation video can be accessed via the [link](https://youtu.be/JfaxBythV4Q).

Contact him via [LinkedIn](https://www.linkedin.com/in/ed-felten-275171/) or [Twitter](https://twitter.com/EdFelten).

**Louis Guthmann:**

Ecosystem Lead at StarkWare \[[Webpage](https://starkware.co/about-us/)\]

![](https://miro.medium.com/max/1400/0*gqSzMpIgNSD7Xbqd)

He gives a presentation on _L2s and settlement layer: what one needs?_ The presentation video can be accessed via the [link](https://youtu.be/aPdRBjyKjiA).

Contact him via [LinkedIn](https://www.linkedin.com/in/louisguthmann/) or [Twitter](https://twitter.com/GuthL).

**Matt Shams:**

CEO of Blockswap Labs \[[Crunchbase](https://www.crunchbase.com/person/matt-shams-anis)\]

![](https://miro.medium.com/max/1400/0*2CL5iaZ85hbFpxM5)

He gives a presentation on _ETH as a long term collateral for rollup centric future_. The presentation video can be accessed via the [link](https://www.youtube.com/watch?v=6FmiXi1L1Z0).

Contact him via [LinkedIn](https://www.linkedin.com/in/mattshams/) or [Twitter](https://twitter.com/daoboymatt).

3\. Blockchain Consensus
========================

**Andres Elowsson:**

Post-doc at KTH Royal Institute of Technology

![](https://miro.medium.com/max/632/0*08AZOBk5e30CoH2c)

He gives a presentation on _Notes on Ethereum’s circulating supply equilibrium and the prospect of perpetual deflation via minimum viable issuance under proof of stake_. The presentation video can be accessed via the [link](https://youtu.be/LtEMabS0Oas).

Contact him via [LinkedIn](https://www.linkedin.com/in/anders-elowsson-38894a44/).

**David Tse:**

Thomas Kailath and Guanghan Xu Professor at Stanford University School of Engineering \[[Webpage](https://tselab.stanford.edu/)\]

![](https://miro.medium.com/max/1000/0*Dax6JBO73hBc0VI8)

He gives a presentation on _Reducing stake lockup period via Bitcoin timestamping_. The presentation video can be accessed via the [link](https://www.youtube.com/watch?v=RmM0TxYiyZg).

Contact him via [LinkedIn](https://www.linkedin.com/in/david-tse-01656774/) or [Twitter](https://twitter.com/dntse).

**Joachim Neu:**

4th year Ph.D. student at Stanford working with David Tse \[[Webpage](https://www.jneu.net/)\]

![](https://miro.medium.com/max/600/0*KuZFLiNHArGXkY__)

He gives a presentation on _The Why and How of PoS Ethereum’s Consensus Problem_. The presentation video can be accessed via the [link](https://www.youtube.com/watch?v=2nMS-TK_tMw).

Contact him via [Twitter](https://mobile.twitter.com/jneu_net).

**Sreeram Kannan:**

Assistant Professor at the University of Washington, Seattle, Director of UW-Blockchain-Lab \[[Webpage](https://people.ece.uw.edu/kannan_sreeram/)\]

![](https://miro.medium.com/max/600/0*Ju4_tQUHqdIUIUzQ)

He gives a presentation on _EigenLayr: Permissionless Feature Addition to Ethereum_. The presentation video can be accessed via the [link](https://www.youtube.com/watch?v=01xDSwMO5U4).

Contact him via [LinkedIn](https://www.linkedin.com/in/sreeram-kannan-a397a47/) or [Twitter](https://twitter.com/sreeramkannan).

4\. Cryptoeconomics
===================

**Guillaume Felley:**

Software Engineer at Reflexer Lab \[[Webpage](https://guillaume.felley.io/)\]

![](https://miro.medium.com/max/800/0*-0FNhPFu_W-T3Twz)

He gives a presentation on _PID control & Cryptoeconomics_. The presentation video can be accessed via the [link](https://youtu.be/2tq5dWNdBXY).

Contact him via [LinkedIn](https://www.linkedin.com/in/guillaume-felley-10514140/) or [Twitter](https://twitter.com/guifel_).

**Irina Katunina:**

Team lead of Analytics at Lido Finance \[[Webpage](https://blog.lido.fi/author/irina/)\]

![](https://miro.medium.com/max/800/0*_9vO1cMBzy6bsKgC)

She gives a presentation on _Modeling the entry queue post Merge: an analysis of impacts on Lido’s “socialized model”_. The presentation video can be accessed via the [link](https://www.youtube.com/watch?v=AjL49bvZ90M).

Contact her via [LinkedIn](https://www.linkedin.com/in/irina-katunina-a98285210/) or [Twitter](https://twitter.com/ikatunya).

**Ross Eyre:**

Transdisciplinary designer & software engineer at ARKOLOGY

![](https://miro.medium.com/max/1400/0*WQO-neCfU7Dyg5Vi)

He gives a presentation on _Modelling Ethereum: Introduction to System Dynamics_. The presentation video can be accessed via the [link](https://www.youtube.com/watch?v=VynhT3qdT-A).

Contact him via [LinkedIn](https://www.linkedin.com/in/rosseyre/) or [Twitter](https://twitter.com/rosseyre).

**Tom Mellan:**

Research scientist at Protocollabs \[[Webpage](https://research.protocol.ai/authors/tom-mellan/)\]

![](https://miro.medium.com/max/798/0*UOkZhylOll1gCXm7)

He gives a presentation on _Filecoin x Ethereum: Introduction to Filecoin CryptoEconomics and Relevance to Ethereum_. The presentation video can be accessed via the [link](https://www.youtube.com/watch?v=36f1GMlYMKw).

Contact him via [Twitter](https://twitter.com/mellantom).

5\. Game Theory
===============

**Bruno Mazorra:**

2nd year Ph.D. student at the University of Pompeu Fabra

![](https://miro.medium.com/max/322/0*nwgTrxX5wHWDTWmG)

He gives a presentation on _Is Folk’s theorem the Blockchain’s nightmare?_ The presentation video can be accessed via the [link](https://www.youtube.com/watch?v=WsrzWuA0xdo).

Contact him via [LinkedIn](https://www.linkedin.com/in/bruno-mazorra-305360120/).

**Philipp Zahn:**

Assistant Professor School of Economics and Political Science at the University of St. Gallen \[[Webpage](https://www.philipp-zahn.com/)\]

![](https://miro.medium.com/max/600/0*ZMm5H9WeqTcmo6D6)

He gives a presentation on _Compositional Game Theory_. The presentation video can be accessed via the [link](https://youtu.be/fucygCyCyo8).

Contact him via [LinkedIn](https://www.linkedin.com/in/philipp-zahn-39470a56/).

Event organizer/coordinator
===========================

**Barnabé Monnot:**

Research scientist @ Robust Incentives Group, Ethereum Foundation \[[Webpage](https://barnabemonnot.com/)\]

![](https://miro.medium.com/max/1120/0*_4sd53P7WhIPL1gi)

Contact him via [LinkedIn](https://www.linkedin.com/in/barnabemonnot/) or [Twitter](https://twitter.com/barnabemonnot).

Acknowledgments
===============

We appreciate the Ethereum Foundation for hosting this research talk at ETHconomics @ Devconnect 2022.

Executive Editor: Zesen Zhuang

Associate Editor: Xinyu Tian

Chief Editor: Prof. Luyao Zhang

Design: Yixuan Li

About the Author
================

Tianyu Wu, an upcoming senior Math student at Duke Kunshan University (DKU), full admission scholarship recipient, and 2019–2020 National Scholarship recipient. He is an interdisciplinary researcher with his interest and research experiences in blockchain and cryptocurrency, game theory. He once served as the student project leader of “How FinTech Empowers Asset Valuation: Theory and Applications” for the Summer Research Scholar Program at Duke Kunshan University in 2021. He is also the Interim Chair of Human Resources in SciEcon CIC, leading the development of the HR management system in the era of digital transformation.

![](https://miro.medium.com/max/1400/0*IN8SylnN39nC-RSi)<br />Figure  8: Tianyu Wu

Contact him on [LinkedIn](https://www.linkedin.com/in/tianyu-henry-wu/) or [Twitter](https://twitter.com/TianyuHenryWu).
