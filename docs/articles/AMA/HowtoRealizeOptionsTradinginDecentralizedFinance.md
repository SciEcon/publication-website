How to Realize Options Trading in Decentralized Finance
=======================================================

The AMA Interview for Dr. Diana Gamborino-Schweizer
===================================================

**About Dr. Diana Gamborino-Schweizer:**
========================================

![](https://miro.medium.com/max/1400/1*5BOR_tDzO9Ge0sptqXrGcQ.jpeg)<br />Figure  1: Dr. Diana Gamborino-Schweizer

Dr. Diana Gamborino recently joined [Bochsler Finance Solutions AG](https://bochslerfinance.com/homepage/) where she works as a Junior Analyst using her unique background to do research and eventually develop the tokenomics of Decentralized Finance (DeFi) applications. Born and raised in Mexico, Diana received her Ph.D. in Physics in 2019 from the University of Bern, Switzerland where she collaborated in space projects from [ESA](https://www.esa.int/), [NASA](https://www.nasa.gov/), and [JAXA](https://global.jaxa.jp/). Diana is a versatile, professional with comprehensive experience in conceptualizing, leading, and managing interdisciplinary scientific and retail industry projects. Her research has focused on modeling and simulating diverse astrophysical phenomena and using novel computer algorithms to analyze astrophysical data — results of which she has published in diverse scientific journals. She is mainly interested in the area where applied mathematics, programming, quantitative modeling, and data science meet especially in the context of complex systems.

Learn more about Dr. Gamborino, you could follow her via [LinkedIn](https://www.linkedin.com/in/diana-gamborino-phd-a1b4a75a/).

AMA Interview Video
===================

Watch our AMA interview for Dr. Gamborino on our [SciEcon YouTube Channel](https://www.youtube.com/channel/UCQOvF-D45s09FlajFkKzoOA)：

<br />Figure  2: AMA Interview for Dr. Gamborino

Read the Interview Scripts with annotations and references:

Question 1
==========

**Tianyu:**

> I notice that hedging and speculation are two main features of options. Do you think that the decentralized platform [Hegic](https://www.hegic.co/) exists to encourage sustainable investment?

![](https://miro.medium.com/max/1400/1*de1wQzLU38nZyaXkJcNxOA.jpeg)<br />Figure  3: [Hegic](https://static.cryptobriefing.com/wp-content/uploads/2020/09/02092727/Hegic-Cover-Image.jpg)

**Dr. Gamborino:**

> **This question allows for different levels of interpretation given the wide spectrum of what “sustainable investment” can signify, and I think it is better to decompose the question into three different levels.**

> (1) Is using [ETH](https://ethereum.org/en/) as a medium of exchange contributing to sustainable investment practices?
> 
> Environmentally speaking, ETH has proven to be much more adaptive to ecological considerations when compared to its older brother [Bitcoin](https://bitcoin.org/en/) and can be expected to gain even more ground in the future. Economically speaking, its high volatility hinders its use as a medium of exchange so this is an aspect that we would have to see if it persists into a much more mature ETH market. In terms of governance, assuming its protocol continues to work as its founder intended, I think Hegic is a world-class sustainable investing medium, owing to its decentralized nature.
> 
> (2) Is the options trade contributing to the sustainability of the financial market?
> 
> As far as I could go in my research, while classical considerations in option pricing do not consider an interaction between option trades and the price development of the underlying asset price, there is evidence that shows how option trading influences the pricing of the underlying asset [(Ni et al., 2016)](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=2820264). If option trading is shown to reduce the volatility of the underlying asset, then I think it could positively contribute to the role Ethereum plays in sustainable investing.

![](https://miro.medium.com/max/1400/1*u6rly8nRDWVKqV0fKBvDnA.jpeg)<br />Figure  4: [Sustainable Investment](https://media.bizj.us/view/img/11028202/gettyimages-sustainable-investing*1200xx6500-3656-0-311.jpg)

> (3) Does Hegic encourage sustainable investing?
> 
> Hegic’s fundamental assumption is that in the long run, the returns obtained by liquidity providers beat the returns of solo options writers. Therefore, to properly evaluate the sustainability of Hegic, it is necessary to analyze the incentives given to liquidity providers and extrapolate if they are viable in the long run. For this, I found a recent [article](https://albaronventures.com/hegic-analysis-report/) demonstrating this exact analysis and the author found that current data from Hegic suggest that pooled exposure for option sellers isn’t sustainable if they have to rely strictly on the earned premiums. This leads to the conclusion that Hegic’s future success depends on a tokenomics upgrade that would involve either a revenue redistribution from the stakers to Liquidity Providers or an insurance fund to cover their losses.

**Question 2**
==============

**Tianyu:**

> What are the potential risks and bugs in the smart contract of this decentralized derivatives trading platform, Hegic?

**Dr. Gamborino:**

> The potential risks when using the Hegic Protocol are thoroughly explained in a [Medium article](https://medium.com/hegic/hegic-protocol-risks-breakdown-d3dcf8c85d01) written by Hegic itself. To summarize, risks native to the protocol design include potential losses on selling options as a liquidity provider and inability to withdraw funds when liquidity pools are maxed out, and loss of profits when you forget to exercise your options because that is not automated. Other potential risks are due to errors in the currency price feeds provided by [Chainlink](https://zh.chain.link/).

![](https://miro.medium.com/max/1400/1*ZmvilvAkFgO5TKJHfsjLtw.png)<br />Figure  5: Blockchain Oracles for Hybrid Smart Contracts: [Chainlink](https://assets-global.website-files.com/5f6b7190899f41fb70882d08/5fa2e075cfcf344baa0e9063_chainlink-open-graph-images_home%20(with%20illustration).png)

> On the other hand, bugs are practically inherent to any smart contract from any DeFi protocol. For Hegic in particular, we saw how this issue affected the protocol hours after the protocol was launched when a bug in its code locked up $28,000 worth of user funds in the platform’s smart contracts.
> 
> I also did a quick search, and found that Hegic’s participation turned out on the platform called [Immuneﬁ](https://immunefi.com/), a bug bounty platform, detailing the most vulnerable avenues of hacks, bugs, and exploits. Exploring these avenues is necessary since in 2020 alone, hacks and scams cost the Defi community over $238 million in losses. While participation in a bug bounty program is worthy, the rate of the bounties offered by Hegic cap out at $50,000, which can be far below the economic gains offered or the economic loss that can be inflicted by exploiting a potential bug covered by that bounty.

Question 3
==========

**Tianyu:**

> What are the pros and cons of decentralized Option Applications in contrast to the centralized ones? Do you think traditional option trading platforms would migrate to blockchain in the future? What is the rationale behind this trend?

**Dr. Gamborino:**

> To the best of my knowledge, the advantages of decentralized options are inherited from the general pros of DeFi relative to Centralized Finance, i.e. permissionless, trustless. However, there are several challenges or technical limitations of DeFi Options platforms. To mention some, first, expensive gas fees which make frequent trading unsustainable, second, option pricing is complicated and there is no uniﬁed approach, and third, options market cannot exist without a reliable price feed from oracles. These are some issues to be addressed to make it a more attractive approach to blockchain.

Question 4
==========

**Tianyu:**

> What is your motivation for doing research about FinTech and blockchain and why do you decide to become an analyst in FinTech enterprises? Could you provide a case that you apply expertise in previous professional experience to the research in FinTech?

**Dr. Gamborino:**

> To be honest, after withdrawing from my academic career in Physics, I was completely open to the job market. Since I am curious about many topics, I found many possibilities. However, the important criteria for my new job were that I could apply my background on an exciting and modern topic, as well as find the right people to work with. FinTech turned out to be most of this and more! I also met with a great team with a leader with a similar background in Physics and matching work values.
> 
> I haven’t used my expertise to research in FinTech yet but the first time I learned about how my background could be applied to study ﬁnance was while I was doing my masters. At that time, I was working on studying the transport of heat in the [solar corona](https://spaceplace.nasa.gov/sun-corona/en/) which is a highly chaotic system that can be modeled as a stochastic process. My advisor then introduced me to how stock and option prices also follow a stochastic process, which immediately attracted my attention to the topic. Also, during this time, while learning several Machine Learning methods, I discovered that these could be applicable to stock and option pricing, for instance, there are several [scientific papers](https://www.researchgate.net/publication/319476152_Proper_Orthogonal_Decomposition_in_Option_Pricing_Basket_Options_and_Heston_Model) showing how one of the machine learning methods, the Proper Orthogonal Decomposition Method can be used to price options, which is the same method I used when analyzing temperature maps of the solar corona. So there are so many connections and ways I could use my physics and mathematics background in the financial industry.

![](https://miro.medium.com/max/504/1*ZDsiw5FYnDlBJ7ZQMODCfw.jpeg)<br />Figure  6: [Solar Corona](https://spaceplace.nasa.gov/sun-corona/en/)

Question 5
==========

**Tianyu:**

> [Internet computer (IC)](https://dfinity.org/) is the first frictionless blockchain with web speed and internet-scale throughout the world. It extends the functionality of the public Internet so that it can host backend software, transforming it into a global computing platform. How do you think the IC can possibly empower the financial industry? How do you think IC can empower your career in FinTech?

**Dr. Gamborino:**

> I am definitely no expert on IC technology, but as far as I understand, IC could empower the financial industry by using its features to replace the intermediary agents involved in asset management and transactions. While DeFi raised the exciting prospects of cutting out the middleman, the IC has ostensibly a better possibility of replacing the middleman in a more automated way. I think the greatest potential of IC is truly autonomous services. I also think that using IC, the governance of trust funds can be reinvented from a financial perspective, they need much less administration or administration can be automated using IC.
> 
> Now, how I think the IC could empower my career in FinTech is something that is still to be explored as I grow and mature in this industry. We will see in the future, depending on my goals and my ambitions, if that aligns to what I see IC provides.

**Tianyu:**

> Thank you, Dr. Gamborino! Basically, we are together learning from this new technique to empower our possibility in FinTech, so I hope that we can actually come back to further discussion later for the Internet Computer, and try to <br />Figure  out more in our career. Overall, your insight from options and your previous background is very valuable, especially for the young people who are interested in the FinTech area.

**Dr. Gamborino:**

> Thank you very much for your interesting questions, Tianyu, and thanks to the SciEcon organization for facilitating this kind of event. I am very honored to have been part of this session. Last but not least, I would like to thank my husband Florian Schweizer for his incredible support and valuable input in understanding many of the concepts needed to answer the previous questions.

Acknowledgments:
================

Interviewee: Dr. Diana Gamborino

Interviewer: Tianyu Wu

Associate Editor: Zichao Chen

Executive Editors: Tianyu Wu, Xinyu Tian

Advisor and Chief Editor: Prof. Luyao Zhang
