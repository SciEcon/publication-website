A Glance into Liquity
=====================

SciEcon AMA Interview for Dr. Robert Lauko

About Dr. Robert Lauko
======================

![](https://miro.medium.com/max/402/0*4u-R7IC9XNQISz5Y)<br />Figure  1: Dr. Robert Lauko

**Introduction to Dr. Robert Lauko:**

Dr. Robert Lauko is the founder and CEO of Liquity, a leading DeFi lending protocol deployed on Ethereum in April 2021. Liquity is a decentralized borrowing protocol that allows you to draw 0% interest loans against Ether used as collateral. Before founding Liquity, Dr. Lauko worked at DFINITY as a research associate. Having worked on multiple projects, Dr. Lauko accumulates rich industry experience in blockchain and decentralized finance. He holds a Ph.D. in Law from the University of Zurich.

![](https://miro.medium.com/max/1400/1*k3zIoGrn_HLcp-5663kK6w.png)<br />Figure  2: [DKU First Cloud Field Trip To Liquity](https://sites.duke.edu/econ204_001_f2020/field-trip/)

Beyond being an industry pioneer, Dr. Robert has contributed passionately and generously to intellectual conversations. At the end of 2020, despite his busy agenda for launching Liquity, he co-hosted the first cloud field trip with Prof. Zhang at Duke Kunshan University. During these times of Covid disruption, the cloud field trip was an innovative way for DKU students to feel connected with the subjects that they are learning and Dr. Lauko shared his thoughts and experience in an enlightening and entertaining presentation on Interest-Free Borrowing & Stablecoin.

Learn more about Dr. Lauko by following him on [Twitter](https://twitter.com/robert_lauko) and [Linkedin](https://www.linkedin.com/in/robert-lauko).

Interview Recording
===================

Watch our AMA interview for Dr. Robert Lauko on our [YouTube channel](https://youtu.be/Jr_1RScaIvo), SciEcon.

Read the Interview Scripts with annotations and citations.

Questions 1
===========

**William:**

> How did you come up with the idea of Liquity? While many decentralized borrowing protocols have already been developed (MakerDAO \[1\] for example), how does Liquity differ from other borrowing protocols?

**Dr. Lauko:**

![](https://miro.medium.com/max/1400/1*SoFmvt-xHwuMiZEgYDTKvQ.png)<br />Figure  3: [Liquity](https://www.liquity.org/)

> Hey William, thank you for having me. I am pleased to be in this show. Let me start by giving you a bit of background about the story of Liquity. While I was working at DFINITY, I just started looking into DeFi protocols that were available at that time. Among them, of course, MakerDAO but there was also Compound \[2\], and there was a protocol back then called ETHland which later became Aave \[3\]. So those were the protocols that I had a chance to look at that time, and I just realized that they were all interesting, but somehow they weren’t as efficient as maybe they could have been. Because the way they did or still do liquidations is time-consuming or involves fixed discounts when they finally sell the collateral.
> 
> Looking at those systems, I realized that I had my own ideas and potential improvements in mind. How to make liquidations faster and even instantaneous? The idea became more and more concrete over time and in November 2019 I left DFINITY to fully focus on Liquity. I was incredibly lucky that I found my co-founder Rick Pardoe who is based in the UK. Now he is the lead engineer, but back then he was the only core Solidity developer. Even though I started with my own prototype in Solidity, I am not a solidity coder. I was only able to create this prototype, and then Rick took over, and the protocol started to shape up. So basically it all started with the efficiency of liquidations. Later we also added other aspects and benefits including the interest-free-ness.
> 
> We weren’t sure at the beginning whether there would be fees and how we would collect them. It turned out that we didn’t want to have interest rates because they make the loans more unpredictable, we wanted to offer a more predictable and smoother borrowing experience. So the whole system targets the borrowers and is trying to make the borrowing experience as good as possible. So it’s not solely a stable coin project, even though the LUSD token is a stablecoin pegged to the US dollar. You could call the stablecoin a byproduct, though it’s an important one. Still, we are a borrowing protocol at our core. That’s how it all started.

**William:**

> That sounds great! I agree that Liquity definitely provides more benefits than only being a stablecoin and that’s really important. We know that Liquity has been deployed on Ethereum for four months. Are there any updates regarding the protocol? Are you satisfied with the performance of the platform up to now?

**Dr. Lauko:**

![](https://miro.medium.com/max/1400/0*cAr7wFiD6mE7wF3p.png)<br />Figure  4: [Liquity Official Website](https://www.liquity.org/)

> Yes, I was literally blown away by our success in the first few days of our protocol. So we launched on April 5, and within the first 10 days, Liquity reached a TVL \[4\] of more than 1 billion US dollars, which was crazy. I mean, I wouldn’t have even dreamed of that in my wildest dreams. But it happened, and it went up to almost five or five and a half billion US dollars, now it has stabilized around 2.5 billion. So it was an incredible early growth, also thanks to our very radical early adopter incentive program.
> 
> We have the stability pool in our system which backs the loans, and by becoming a stability depositor you also get rewarded in our secondary token LQTY, and the way the system mints and distributes the LQTY by is heavily weighted towards the early adopters. So it made sense for them to jump on as early as possible, which then fuelled the whole system with more fee revenue. That kickstarted the whole cycle. I think the early success of the protocol was extremely important because it also helped us to be in the media and have some echo on Twitter and just make sure that people start talking about Liquity.
> 
> Yeah, I am really happy with how this all worked out because I wasn’t sure at the beginning whether our system will be used. Maybe it could have gone wrong, but it turned out to be successful.

Questions 2
===========

**Xinyu:**

> Thank you so much for sharing your story behind the industry. The pathway is really inspiring to us. In the past year, we see a boom in decentralized finance on the Ethereum blockchain. As an industry practitioner, what do you think about the prospect of DeFi? What are the key advantages of operating on the blockchain compared to a centralized system, and what are the potential disadvantages?

**Dr. Lauko:**

![](https://miro.medium.com/max/1400/0*NJxPZkkc98msJ4N9.jpg)<br />Figure  5: [DeFi](https://www.google.com/url?sa=i&url=https%3A%2F%2Fcoinquora.com%2Ftop-10-defi-lending-platforms-in-2021%2F&psig=AOvVaw2k8qXOjcC7w_9yDSrDpTkV&ust=1634115539770000&source=images&cd=vfe&ved=2ahUKEwif-7bzwMTzAhUHU1MKHXsGBCoQr4kDegUIARCtAQ)

> That’s a great question. There are disadvantages and advantages, of course. I think one of the main advantages is that you can automate things. You can basically do away with intermediaries, with human interaction. So you can make everything more predictable because you can set the rules in stone. You can make sure that by making it transparent, people know exactly what they have to expect — they know exactly when they get liquidated, and they know exactly what they have to pay. I think this really changes the way people interact with financial products. That’s one of the advantages.
> 
> Another advantage is that you can make them much more efficient. There is always an open market for crypto, for example, while the stock market closes on the weekend. Even that shows how much more efficient crypto trading, for example, can be. So I think there are many ways of automating things, making them more efficient and more cost-efficient as well, by cutting out the intermediaries. You have fewer people taking their share, so you can offer the resulting product at a much more attractive price. I think those are the pros.
> 
> On the con side, depending on how the protocol is structured, it can be a problem that decentralized applications are more static. Sometimes a human intervention can be an advantage because humans can adapt to changes that you couldn’t foresee as a protocol developer. So in Liquity it’s not possible at all to change the protocol. In other systems, there may be a governance mechanism, but who knows whether it will decide the way it should. A central entity can lead to a fairer outcome or to results that people would prefer.
> 
> And maybe another advantage of centralized exchanges is the human aspect, the fact that you as a human can interact with other humans. Some people may prefer having a partner whom they can talk to and who is in charge or responsible for a product or service. While in DeFi, this may be less obvious. There are even teams that are fully anonymous or products that just live on by themselves, without having an owner or admin. Or, they are even abandoned, but they still keep working. Some people may be a bit confused and would not trust such a system. So, there are pros and cons for sure.

Questions 3
===========

**William:**

> I totally agree, I think your insights about the pros and cons of DeFi are really important to us. The third question is that there are already different versions of Liquity deployed on various blockchains (Binance Smart Chain (BSC) for example). There are also projects aiming to deploy Liquity to Internet Computer (IC). What do you think about the prospects of these public blockchains?

**Dr. Lauko:**

> I think we have to differentiate between the future of those blockchains as infrastructure projects and the future of DeFi. Because I think some newer blockchain protocols have a much broader use case or scope than just DeFi.
> 
> An important presentation given by Vitalik Buterin in Paris, a few weeks ago at the EthCC, made it clear that Ethereum shouldn’t be just about DeFi, because blockchains could offer much more than financial products; they could also tap into the social media space, for example. And I think that was a very interesting talk because that’s what other blockchains are now currently pursuing and maybe they are more advanced in that sense than Ethereum. For example, DFINITY is pushing the boundaries of being scalable and much faster and cost-efficient than Ethereum. We have already seen some interesting applications being built on top of DFINITY that would be never possible technically on Ethereum.
> 
> And there is also Solana, which is targeted to become more efficient than Ethereum. Then the question is: do we need all the efficiency and scalability for DeFi? And this is a difficult question. I think even though Ethereum has its issues with the gas costs, it’s slow and can only evolve through hard forks, but it already has a thriving DeFi ecosystem on Ethereum. And while it may not be optimal, it still works.
> 
> And the question is, would it become much better if we move to more efficient chains? Here I’m not sure. I think it depends on the application, in particular. For example, the way the decentralized exchanges are designed now on Ethereum is influenced by Ethereum’s low throughput and low scalability. That’s why we only have pool-based systems like Uniswap for token exchanges, because you cannot replicate order-book \[5\] based dynamics or a traditional trading platform on Ethereum. It just doesn’t work because it’s too slow and it would be too expensive. But now, with DFINITY, I think that would become possible and maybe we will also see more order-book based systems pop up in the future.
> 
> Now Liquity is a bit of a different story, because Liquity is a loan platform. It’s a borrowing protocol, where users would take out a loan, but only change the loan like repaying some portion or take out more, maybe every week or month or not even that often. So maintaining a loan is not the same as being a trader. The traders may do 10 trades a day or even 100 trades or more. For them, speed and cost efficiency are much more important than for a borrower on Liquity, who may not care too much: you could open your position and maybe in a year you repay. That’s why our strategy around layer two solutions and other chains is not very urgent for now. We don’t feel a pressing need to be everywhere and to make sure that people can open Liquity loans on every layer 2 chain, because I don’t think there is a very clear need for it. But of course it would be nice to eventually offer that.
> 
> Maybe I can quickly come back to the last part of your first question, because I’m not sure if I answered it. We just recently started working on a second project that could extend the scope of Liquity as a native stablecoin borrowing system. On Compound, for example, you can borrow existing tokens and you can collateralize them with other existing tokens. We want to create something similar, but without charging an interest rate. It would be similar to Liquity in the fact that there is no interest rate but some upfront fee that you pay when you take out your loan and that’s it.
> 
> While we were working on this idea, we also realized that this kind of idea could also benefit the current ecosystem of Liquity. And we could also do it in a way to make it work on multiple different chains. Ideally, we could deploy it to several networks once implemented, but we don’t need to decide this for the time being.

**William:**

> Thank you Dr. Lauko, it’s really great to hear that there might be Liquity version two or Eureka as you mentioned. I think this is really exciting information for us. I totally agree that this is a great idea. I think it will help us a lot to improve the user experience when users can not only use Ethers as collateral but also other tokens. So that’s all of our questions. Thank you so much for taking us into our interview today, and thank you so much for providing us with these insights.

**Dr. Lauko:**

> Thank you for this great interview, it was a pleasure to be here. Great, thank you for inviting me.

Relevant Materials
==================

\[1\] MakerDAO

The Maker Protocol, also known as the Multi-Collateral Dai (MCD) system, allows users to generate Dai by leveraging collateral assets. Dai is a decentralized, unbiased, collateral-backed cryptocurrency soft-pegged to the US Dollar.

[Website](https://makerdao.com/en/), [Whitepaper](https://makerdao.com/en/whitepaper)

\[2\] Compound

The compound is a protocol on the Ethereum blockchain that establishes money markets, which are pools of assets with algorithmically derived interest rates, based on the supply and demand for the asset.

[Website](https://compound.finance/), [Whitepaper](https://compound.finance/documents/Compound.Whitepaper.pdf)

\[3\] Aave

Aave is an open-source and non-custodial liquidity protocol for earning interest on deposits and borrowing assets. It shifts from a decentralized P2P strategy to a pool-based strategy.

[Website](https://aave.com/), [Whitepaper](https://github.com/aave/protocol-v2/blob/master/aave-v2-whitepaper.pdf)

\[4\] TVL (Total Value Locked)

Total Value Locked (TVL) represents the number of assets that are currently being staked in a specific protocol. It is a metric that is used to measure the overall health of the DeFi and yielding market. You can track total value locked on many services.

[Article on Messari](https://messari.io/article/how-to-interpret-total-value-locked-tvl-in-defi) [on CoinMarketcap](https://coinmarketcap.com/alexandria/glossary/total-value-locked-tvl)

\[5\] order book

An order book is an electronic list of buy and sell orders for a security or other instrument organized by price level. Order books are used by traditional financial exchange for various assets like stocks, bonds, currencies, and even cryptocurrencies.

[Investopedia](https://www.investopedia.com/terms/o/order-book.asp)

Acknowledgments:
================

Interviewee: Dr. Robert Lauko

Interviewers: Xinyu Tian, William Zhao

Executive Editors: William Zhao, Xinyu Tian

Advisors and Chief Editors: Prof. Luyao Zhang and Prof. Yulin Liu
