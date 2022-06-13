WaterPark: A Decentralized  
Borrowing Protocol for the Internet Computer
=========================================================================

The AMA Interview for Duke CS+ Project Waterpark team
-----------------------------------------------------

> Disclaimer: this interview documentary is an extension of the Duke CS+ Project Summer 2021 entitled “[Decentralized Finance: Blockchain and Cryptocurrency on the Internet Computer](https://www.cs.duke.edu/undergrad/summer_research).” Inspired by [Prof. Campbell Harvey](https://medium.com/sciecon-ama/how-will-defi-reshape-the-future-of-finance-a5febf668487)’s initiatives in DeFi, we are developing research-oriented DeFi Applications on the Internet Computer. The project lead is [Prof. Luyao Zhang](https://www.linkedin.com/in/sunshineluyao/), Senior Research Scientist at Data Science Research Center and Assistant Professor of Economics at Duke Kunshan University. The co-leads include [Prof. Kartik Nayak](https://users.cs.duke.edu/~kartik/) and [Prof. Fan Zhang](https://www.fanzhang.me/), Assistant Professor of Computer Science at Duke University and industry pioneer [Prof. Yulin Liu](https://www.linkedin.com/in/yulineth/), the Partner and Head of Research at [Bochsler Finance](https://bochslerfinance.com/about-us/) and Chief Economists for several DeFi projects. The research team includes graduate mentor [Derrick Adam](https://www.linkedin.com/in/derrick-adam/), a master’s student from the Economics and Computer Science program, and undergraduate researchers [Dylan Paul](https://www.linkedin.com/in/dylanpaul1/), [Malika Rawal](https://www.linkedin.com/in/malika-rawal-303140160/), [Oum Lahade](https://www.linkedin.com/in/oum-lahade-920b30177/), and [Urjit Banerjee](https://www.linkedin.com/in/urjit-banerjee-81210718b/) at Duke University. The undergraduate researchers have a diverse background in computer science, finance, electrical & computer engineering, mathematics, etc.
> 
> Our team embodies the spirits of diversity and inclusion in research, innovation, and leadership. We collaborate across genders, nationalities, disciplines, industries, institutions, time zones, and much more.
> 
> We acknowledge [Prof. Brandon Fain](https://sites.duke.edu/btfain/), [Prof. Robert Calderbank](https://ece.duke.edu/faculty/robert-calderbank), and [Prof. Jun Yang](https://users.cs.duke.edu/~junyang/) for their initial organization that made this project possible. We are also grateful for the support from DFINITY and student volunteers from Duke Kunshan University.

About the Interviewees
======================

**Introduction to Rhys Banerjee**

![](https://miro.medium.com/max/344/1*AbEjgkzJpVi03nIvTJhIFA.png)<br />Figure  1: Rhys Banerjee

Rhys is a rising Junior at Duke University currently majoring in Computer Science and minoring in Mathematics. Since June 1st he has been on the Decentralized Finance team at the CS+ program at Duke. They have been leveraging the Internet Computer to build a decentralized undercollateralized lending protocol consisting of an exchange of ICP to an SDR-pegged stablecoin. This project has taught him much about both coding, collaboration, and academic research into the field of blockchain, which I was initially mostly unfamiliar with.

**Introduction to Oum Lahade**

![](https://miro.medium.com/max/684/1*o_dgITslpGwT7gyZZA-x-w.png)<br />Figure  2: Oum Lahade

Oum is a rising Sophomore at Duke University studying Electrical & Computer Engineering and Mathematics with a minor in Finance. This summer, he has been working to create a decentralized borrowing protocol called WaterPark, modeled off the Liquity protocol on Ethereum, on the Internet Computer. Learning about the Internet Computer has taught him a lot about blockchain and various innovations within the field while developing the protocol has endowed him with greater teamwork and project management skills.

Watch the interview documentary on [SciEcon YouTube channel](https://youtu.be/YpJCpcUuVBs):

Read the Interview Scripts with annotations and citations.

Questions 1
===========

**Xinyu:**

> We know that you have joined the Duke CS+ group and are working on a project named WaterPark related to the Internet Computer and distributed finance, so can you please give us a brief introduction to your project, including its expectation and objectives?

**Oum:**

> Sure, I can start. So WaterPark is a decentralized borrowing protocol on the Internet Computer \[1\] Network, which is modeled off the Liquity \[2\] protocol on Ethereum \[3\]. So here the general idea is that the user will deposit ICP \[4\] tokens, which are the native tokens of the Internet Computer, into these things, called Troves, which are essentially debt accounts, on WaterPark. And after they deposit ICP tokens on WaterPark they will be able to take out a stable coin, pegged to the SDR \[5\], that is over collateralized from the system. And so the idea here is that they can use the stable coin to create stable smart contracts or canisters \[6\] on the Internet Computer Network while still having the price appreciation that ICP tokens offer.

![](https://miro.medium.com/max/768/1*QacLAei1d1c1QoRLEXb6ug.png)<br />Figure  3: [Liquity](https://www.liquity.org/)

**Xinyu:**

> So Rhys, do you want to add something?

**Rhys:**

> Yeah. There’s not really much to add beyond that, I mean I feel like he pretty much covered the essentials of WaterPark. It is based on the already existing Liquity protocol, but we had to make a few adaptations, just in terms of using ICP tokens instead of Ether tokens. And we’re going to be implementing our own stable coin \[7\] pegged to Internet Computer cycles, as opposed to the LUSD \[8\] stable coin for Liquity. But I feel like Oum has pretty much covered everything.

Questions 2
===========

**Zesen:**

> Thank you so much. So as you said, unlike most of the theoretical learning that takes place in the university courses, the project you’re working on is such an integrated activity that combines research and technical practice. So, could you please briefly talk about your incentives for starting this project and did this kind of project help you in your studies or in your future career?

**Rhys:**

> So I am actually not from a finance background, I am more from a computer science or math background, and I am more like an amateur with an interest in blockchain. In terms of my interest in this project, I was interested mainly because we were going to be working with new technologies like the Internet Computer. And I was interested in the prospects of making a DeFi \[9\] protocol on this level of technology.

![](https://miro.medium.com/max/902/1*amgJ7upybs2hWmKG-PuMnw.png)<br />Figure  4: [Defi protocols](https://medium.com/alethio/the-defi-series-an-overview-of-the-ecosystem-and-major-protocols-da27d7b11191)

**Oum:**

> This project essentially stemmed from a previous interest in blockchain, as well as, just understanding Defi architecture which I think is a huge thing going forward. And then, how this project help in our future career? I think, for me, it’s pretty much just been eye-opening to see a new side of finance that’s currently in development, which stands in contrast to a lot of other areas of finance.

Questions 3
===========

**Xinyu:**

> Cool. So as you have taken two months into the Duke CS+ project, can you give a brief overview of how the project is proceeding so far, or can you share something like your significant achievements that you have already reached?

**Oum:**

> Sure. So on the development side, we created an MVP \[10\] (Minimum Viable Product) a few weeks back, and we’ve been refining that and sort of getting that more integrated within the whole Internet Computer network. And then on the research side, we’re currently in the midst of developing our further research proposal, which for both of us revolves around the idea of orthogonal persistence \[11\] which is something that Dfinity is implemented in a novel way on the Internet Computer.

![](https://miro.medium.com/max/800/1*lbmM1qvNcqt1fBx64-fCUA.png)<br />Figure  5: [Orthogonal Persistence](https://charted.space/orthogonal-persistence.html)

> And so, those have been the two main accomplishments that we have obtained so far.

**Rhys:**

> Pretty much as Oum said, we have the minimum viable product and we’re also now in the midst of just finalizing our research proposals. My research proposal focuses more on orthogonal persistence as a solution to data storage and Oum focuses more on orthogonal persistence as a solution to efficiency. So our research proposals are similar and a little bit different. That’s pretty much where we are right now in terms of the project as a whole.

**Xinyu:**

> Congratulations on all your achievements!

Questions 4
===========

**Zesen:**

> Thank you so much. I think this would be the last question of this interview, which said that you are now working in a completely new field and the technology stack you’re using is very new, such as the Motoko programming language, etc. And relatively speaking, these technologies often do not have a very mature ecology, which means that information retrieval can be very difficult. Have you ever encountered similar problems in your research and how did you resolve them?

**Rhys:**

> I can speak a little bit to some difficulties that sound more from the fact that the Internet Computer and Motoko \[12\] are new , which pretty much means that if you run into any sort of issue, there is a large likelihood that you can’t just Google the problem and find some solution on StackOverflow or some other website. I am trying to come up with specifics, but I just know that I have a lot. But I know that one of them that I am encountering right now is issues with the frontend. Me and Malika who is on the other project of the DeFi, we’re running into some issues connecting the frontend and the backend into a cohesive product. And I guess the only solution that is presented right now is contacting other DFinity developers. Because when the technology is so new and the only solution that you can really find is finding other people who are developing on the Internet Computer, you need to come up with some sort of support network.

**Oum:**

> Yeah and I think I can speak to a very similar experience, as recently as you mentioned earlier the Motoko ecology is not very developed yet. So because of that, the documentation can be at times kind of lacking. For me, most of the problems that I encountered were with the actual integration on the Internet Computer. For example, actually transferring ICP tokens between wallets, or creating a new stable coin and having a canister for that.

![](https://miro.medium.com/max/558/1*eh-hNmt32jH0jadYfAu4JA.png)<br />Figure  6: Token transfer

> For that, as previously mentioned, the workarounds for that come from posting on the Dfinity forums or talking to different engineers, and I know our CS+ professor has given us the opportunity to submit questions for an AMA which I think should be helpful as well.

**Rhys:**

> That’s true.

**Xinyu:**

> Thank you so much, and I guess this is the end of our interview, so thank you for your participation and we’re so looking forward to your future achievement and also other collaborations between DKU and Duke. So thank you so much.

Relevant Materials
==================

\[1\] Internet Computer

Developed by DFINITY Foundation, the Internet Computer extends the functionality of the public Internet so that it can host backend software, transforming it into a global computing platform. Using the Internet Computer, developers can create websites, enterprise IT systems, and internet services by installing their code directly on the public Internet and dispensing with server computers and commercial cloud services.

[Website](https://internetcomputer.org/), [Medium](https://medium.com/dfinity)

\[2\] Liquity

Liquity is a decentralized borrowing protocol that allows you to draw 0% interest loans against Ether used as collateral. Loans are paid out in LUSD — a USD pegged stablecoin, and need to maintain a minimum collateral ratio of only 110%.

[Website](https://www.liquity.org/)

\[3\] Ethereum

Ethereum is a decentralized, open-source blockchain with smart contract functionality. Ether (ETH or Ξ) is the native cryptocurrency of the platform. After Bitcoin, it is the largest cryptocurrency by market capitalization. Ethereum is the most actively used blockchain.

[Website](https://ethereum.org/en/), [Wikipedia](https://www.investopedia.com/terms/l/legal-tender.asp)

\[4\] ICP

The ICP token is designed to help operate a decentralized layer of web infrastructure being built by DFinity that believers say will liberate users from reliance on companies like Amazon and Google.

[Website](https://www.nytimes.com/2021/06/28/business/dealbook/icp-cryptocurrency-crash.html#:~:text=The%20ICP%20token%20is%20designed,companies%20like%20Amazon%20and%20Google.)

\[5\] SDR

The SDR is an international reserve asset, created by the IMF in 1969 to supplement its member countries’ official reserves. So far SDR 204.2 billion (equivalent to about US$293 billion) have been allocated to members, including SDR 182.6 billion allocated in 2009 in the wake of the global financial crisis. The value of the SDR is based on a basket of five currencies — the U.S. dollar, the euro, the Chinese renminbi, the Japanese yen, and the British pound sterling.

[Website](https://www.imf.org/en/About/Factsheets/Sheets/2016/08/01/14/51/Special-Drawing-Right-SDR)

\[6\] Canister

A canister is a conceptual object similar to a smart contract with a universally-unique identifier and an owner that defines the boundaries of a specific application, service, or micro-site. A canister encapsulates all of the programming logic, public entry methods, the interface description for the provided message types, and state information for the application, service, or micro-service it describes.

[Website](https://sdk.dfinity.org/docs/developers-guide/glossary.html)

\[7\] Stable Coin

Stablecoins are cryptocurrencies where the price is designed to be pegged to a cryptocurrency, fiat money, or to exchange-traded commodities (such as precious metals or industrial metals).

[Wikipedia](https://en.wikipedia.org/wiki/Stablecoin)

\[8\] LUSD

Liquity USD (LUSD) is the USD-pegged stablecoin used to pay out loans on the Liquity protocol. At any time it can be redeemed against the underlying collateral at face value. … Loans are paid out in LUSD — a USD pegged stablecoin, and need to maintain a minimum collateral ratio of only 110%.

[Website](https://morioh.com/p/cf283f91beb9)

\[9\] DeFi

DeFi is an open and global financial system built for the internet age — an alternative to a system that’s opaque, tightly controlled, and held together by decades-old infrastructure and processes. It gives you control and visibility over your money. It gives you exposure to global markets and alternatives to your local currency or banking options. DeFi products open up financial services to anyone with an internet connection and they’re largely owned and maintained by their users. So far tens of billions of dollars worth of crypto have flowed through DeFi applications and it’s growing every day.

[Website](https://ethereum.org/en/defi/)

\[10\] MVP

A minimum viable product (MVP) is a version of a product with just enough features to be usable by early customers who can then provide feedback for future product development.

[Wikipedia](https://en.wikipedia.org/wiki/Minimum_viable_product#:~:text=A%20minimum%20viable%20product%20(MVP,and%20(ultimately)%20unnecessary%20work.)

\[11\] Orthogonal Persistence

In Internet Computer, developers don’t have to think about persistence — they just write their code and persistence happens automatically. It’s called orthogonal persistence. Persistence is said to be “orthogonal” or “transparent” when it is implemented as an intrinsic property of the execution environment of a program. An orthogonal persistence environment does not require any specific actions by programs running in it to retrieve or save their state.

[Website](https://medium.com/dfinity/a-technical-overview-of-the-internet-computer-f57c62abc20f), [Wikipedia](https://en.wikipedia.org/wiki/Persistence_(computer_science)#:~:text=8%20References-,Orthogonal%20or%20transparent%20persistence,retrieve%20or%20save%20their%20state.)

\[12\] Motoko

Motoko is a programming language that is designed to seamlessly support the programming model of the Internet Computer, making it easier to efficiently build applications and take advantage of some of the more unique features of the platform. Motoko is strongly typed, actor-based, and has built-in support for orthogonal persistence and asynchronous message passing. Productivity and safety features include automatic memory management, generics, type inference, pattern matching, and both arbitrary- and fixed-precision arithmetic. Messaging transparently employs the Internet Computer’s Candid interface definition language and wire format for typed, high-level, and cross-language interoperability.

[Website](https://dfinity.org/technicals/motoko)

Acknowledgments:
================

Interviewee: Rhys Banerjee, Oum Lahade

Interviewer: Xinyu Tian, Zesen Zhuang

Associate Editor: Lunji Zhu

Executive Editors: Xinyu Tian, Zesen Zhuang

Chief Editor: Prof. Luyao Zhang
