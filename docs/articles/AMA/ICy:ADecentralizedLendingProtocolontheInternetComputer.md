ICy: A Decentralized Lending Protocol on the Internet Computer
==============================================================

The AMA Interview for Duke CS+ Project ICy team
-----------------------------------------------

> Disclaimer: this interview documentary is an extension of the Duke CS+ Project Summer 2021 entitled “[Decentralized Finance: Blockchain and Cryptocurrency on the Internet Computer](https://www.cs.duke.edu/undergrad/summer_research).” Inspired by [Prof. Campbell Harvey](https://medium.com/sciecon-ama/how-will-defi-reshape-the-future-of-finance-a5febf668487)’s initiatives in DeFi, we are developing research-oriented DeFi Applications on the Internet Computer. The project lead is [Prof. Luyao Zhang](https://www.linkedin.com/in/sunshineluyao/), Senior Research Scientist at Data Science Research Center and Assistant Professor of Economics at Duke Kunshan University. The co-leads include [Prof. Kartik Nayak](https://users.cs.duke.edu/~kartik/) and [Prof. Fan Zhang](https://www.fanzhang.me/), Assistant Professor of Computer Science at Duke University and industry pioneer [Prof. Yulin Liu](https://www.linkedin.com/in/yulineth/), the Partner and Head of Research at [Bochsler Finance](https://bochslerfinance.com/about-us/) and Chief Economists for several DeFi projects. The research team includes graduate mentor [Derrick Adam](https://www.linkedin.com/in/derrick-adam/), a master’s student from the Economics and Computer Science program, and undergraduate researchers [Dylan Paul](https://www.linkedin.com/in/dylanpaul1/), [Malika Rawal](https://www.linkedin.com/in/malika-rawal-303140160/), [Oum Lahade](https://www.linkedin.com/in/oum-lahade-920b30177/), and [Urjit Banerjee](https://www.linkedin.com/in/urjit-banerjee-81210718b/) at Duke University. The undergraduate researchers have a diverse background in computer science, finance, electrical & computer engineering, mathematics, etc.
> 
> Our team embodies the spirits of diversity and inclusion in research, innovation, and leadership. We collaborate across genders, nationalities, disciplines, industries, institutions, time zones, and much more.
> 
> We acknowledge [Prof. Brandon Fain](https://sites.duke.edu/btfain/), [Prof. Robert Calderbank](https://ece.duke.edu/faculty/robert-calderbank), and [Prof. Jun Yang](https://users.cs.duke.edu/~junyang/) for their initial organization that made this project possible. We are also grateful for the support from DFINITY and student volunteers from Duke Kunshan University.

About the Interviewees
======================

**Introduction to Dylan Paul:**

![](https://miro.medium.com/max/328/1*_5BmbfB1TQ_DErEb15e6cw.png)<br />Figure  1: Dylan Paul

Dylan is a rising Junior at Duke University majoring in Computer Science with a concentration in Machine Learning and minoring in Finance. He is extremely passionate about blockchain technology as well as Decentralized Finance. This summer, he has been working on the Decentralized Finance Team as part of the CS+ program through Duke. As part of this team, he has learned the MOTOKO language as well as the DFINITY architecture to construct an AAVE-like decentralized lending protocol on the Internet Computer. With this application, he hopes to conduct research comparing the reverse gas model to the gas model as seen on Ethereum.

**Introduction to Malika Rawal:**

![](https://miro.medium.com/max/358/1*T1X6eEQ02EH1u3qnz6iulA.png)<br />Figure  2: Malika Rawal

Malika is a rising Sophomore at Duke University studying economics and computer science. She is very interested in the fintech area and has really enjoyed learning about decentralized finance through Duke CS+’s “Decentralized Finance on the Internet Computer” research team. They are learning about utilizing Dfinity’s Internet Computer to build decentralized lending programs, specifically those replicating concepts from Liquity and Compound Aave. She is working with her research partner, Dylan Paul, on replicating Aave and they have created their own project called ICy (Internet Computer Yield). With this application, she hopes to conduct research comparing liquid democracy and governance on the Internet Computer and Ethereum.

Watch the interview documentary on [SciEcon YouTube Channel](https://youtu.be/YpJCpcUuVBs):

Read the Interview Scripts with annotations and references:

Questions 1
===========

**Xinyu:**

> As we participated in the Duke CS+ team in the past two months, we’re really interested in your project. So now we have some questions for you as you’re the researchers in that project. So the first question is that we know that you’ve joined the Duke CS+ program and are working on a project named ICy related to the Internet Computer \[1\] and distributed finance \[2\]. Can you please give us a brief introduction to your project, including its expectations and objectives?

**Malika:**

> ICy stands for Internet Computer yield, and it is a decentralized lending protocol for the Internet Computer. Our inspiration was Aave, which is already on the Ethereum Blockchain, We were trying to follow it in some ways by creating a similar protocol on the Internet Computer, so we did utilize some information from there. In general, that’s the main project that we’ve been working on this semester, but we’ve also been working on our own research projects that we’ve used to improve ICy as well.

![](https://miro.medium.com/max/1400/0*JHpFoYaqOW_C-7Ha)<br />Figure  3: [Decentralized lending protocol](https://www.leewayhertz.com/how-defi-lending-works/)

**Dylan:**

> I think, just to build off that, they’re really two sides to this project. We’ve been working on the research side and the innovation side. For the research side, we all had to come up with our own individual topic but based on the application that we were building, which for us was ICy. And my particular research was targeted towards comparing and analyzing the Ethereum gas model to Dfinity’s Internet Computer’s reverse gas model \[3\] which is really just a fancy way of saying that I’m comparing how transaction fees are working for developers and users on both of these blockchain technologies, and trying to see how these fees affect users and developers economic decisions. So the innovation side enables us to make these comparisons because we were recreating a decentralized lending protocol that resembles Ethereum’s \[4\] AAVE. This means that we’re recreating a decentralized bank protocol with lending and borrowing of crypto assets on the Internet Computer. The name of this application is ICy which stands for Internet Computer Yield, and it will be used to compare the gas models more effectively on both of these platforms.

Questions 2
===========

**Zesen:**

> Thank you so much. Just as you mentioned, unlike most of the theoretical learning that takes place in the university, the project you have been working on is such an integrated activity combining research and technical practice. So could you please briefly talk about your incentives for starting this project and did this project help you with your studies and your future career?

**Dylan:**

> I think for me, I was personally passionate about blockchain technology in general as I’ve interacted with Ethereum and Aave \[5\] and the decentralized applications on their platform. So I thought that this would be a good project to get myself into to start to understand what else is out there in the field. But also, in particular, on Ethereum, a huge problem that they have is the gas fees \[6\]. And as someone that’s a student, I can’t afford to spend so much money on every single transaction that I make. So, I thought it would be really interesting to compare how the gas model differs on Ethereum’s and the Internet Computer’s blockchains. So I think that was my motivation for coming up with that research question and analyzing the difference in the lending protocols, which is what is mostly used on Ethereum.

![](https://miro.medium.com/max/1400/0*qO7jqWkCHrvzv_VJ)<br />Figure  4: [dApps](https://medium.com/hackernoon/what-are-decentralized-applications-dapps-explained-with-examples-7ff8f2c4a460)

**Malika:**

> Similarly, I am an economics and finance student who is also interested in computer science. So I wanted to come in and learn more about the economic side of blockchain and to know what the companies are doing, you can only really know that if you’ve understood the blockchain technologies. So in the past, I’ve invested in various cryptocurrencies but I never even knew how they worked. So I thought this research opportunity would be a good way to see the background of these blockchain companies and understand what’s going on behind the scene. For example, what happens in the background when a company has a pitfall, and what is going on when there is an increase in the crypto’s price. So I think this is a perfect project for me because of my interest in both economics and computer science. When we picked what research we wanted to do, I started with the chain and key technology \[7\], but it was a little bit too broad, because it’s a massive project to handle on IC, so we would take a whole new semester to do. So I narrowed it down to more of the Network Nervous System \[8\], and then liquid democracy. So right now my research paper is on comparing liquid democracy between Ethereum and the Internet Computer so that we can better handle ICy and find a better implementation for it.

Questions 3
===========

**Xinyu:**

> Thank you so much, it’s so nice to see that you’re motivated by your interest and you’re still in progress in what you like. So, two months into the CS+ Project, can you give us a brief overview of how the project is processing so far, like Malika has mentioned a little bit about that, and do you have significant achievements among your project that you can share with us.

**Dylan:**

> I think the biggest achievements that we’ve had came on the backend side recently. We’ve been working on the frontend development to make it look a little bit prettier but the backend was initially difficult to get functioning. Due to the novelty of the Internet Computer, there is not that much documentation out there so learning the language, the syntax and the system was difficult. So I think it is an achievement that we were able to build something that resembles a typical lending protocol. Our ICy protocol enables users to lend and earn interest for providing liquidity, as well as borrow if the users provide enough collateral. There is still more functionality that we can continue to add, but we currently have it working properly for two users. The application also has the ability to scale to more users, but we are keeping it simple for now with two users whose funds we can manually control, which is important for experimentation purposes and therefore our research questions and analysis. So I think the fact that we have a backend that functions as a lending protocol is pretty impressive considering what we were initially given in terms of very little information on what Dfinity really was or the Internet Computer.

**Malika:**

> I agree. I think the backend is definitely the most important part and just learning the language throughout two months is a little bit hard to pick up on because there’s not that much documentation online There are barely any examples out there using Motoko \[9\] or similar languages on the Internet Computer.

![](https://miro.medium.com/max/1400/0*7MLjirq9E9f1G98b)<br />Figure  5: [Motoko Programming Language](https://stackoverflow.blog/2020/08/24/motoko-the-language-that-turns-the-web-into-a-computer/)

> So that would definitely be the biggest one. And then recently I am working on the frontend, we have a baseline nature, and we’re working on integrating the two sides so that we can have it become user compatible. As of right now, we have a front-end demo that can be used to submit grant proposals or advertise our product. It has the main page where a user can play around with the functions, an about page where they can learn about the development of ICy, as well as a developers page where they can learn about the developers, professors, mentors, and research supporters. Also, understanding how to dive in and create specific comparisons in research has been difficult as well. From this summer, I’ve learned a lot about how to do research in economics and computer science and how to pick a specific variable to compare in a study.

Questions 4
===========

**Zesen:**

> I totally understand your pain on the Motoko part because I also write code in this language which lacks documentation. And the last question is also about this field. Say that you are working in a completely new field and the technology stack you are using is very new, such as the Motoko programming language, etc. And relatively speaking, these technologies often do not have a very mature ecology, which means that information retrieval can be very difficult. Have you encountered similar problems in your research and how did you solve them?

**Dylan:**

> For sure, I mean we hit a pretty big roadblock for a little while and we didn’t really know where to turn. We actually consulted Dfinity engineers at one point by reaching out on their developer forum. But it still just wasn’t easy just because of how new the Internet Computer is and there’s no documentation like you said to really draw inspiration from. So we <br />Figure d it out as best as we could and we just continued to tinker, which is, in my opinion, often the best way to <br />Figure  it out, so we just kept on trying and trying. And actually the last couple of nights, we’ve kind of moved from what we had originally to scaling it up a little bit by creating a database type system \[10\] that holds users’ accounts and information, and that kind of overrode some of the problems that we were experiencing earlier. So we’re trying to <br />Figure  out how to get around those problems that we couldn’t really <br />Figure  out at first by trial and error as well as approaching the problem from a different angle.

![](https://miro.medium.com/max/1400/0*jB4JiQuT1ASZbSP5)<br />Figure  6: [Debug](https://geekflare.com/http-client-tools/)

**Malika:**

> Coming from a research standpoint, I think in the beginning, we all picked research topics not really thinking about how to implement them in our code. So some of us had Chain Key Technology, others had reverse gas fee models, orthogonal persistence, there were others as well, but we never really discussed utilizing those concepts to develop similar solutions in our own code. After realizing that was the main intent of the research, we narrowed our research down and focused more on how it can help us with developing ICy . In our research paper, you’ll see a part about how we implement our research on project ICy So that was important because research should go hand in hand with our product.

Relevant Materials
==================

**\[1\] Internet Computer**

Developed by DFINITY Foundation, the Internet Computer extends the functionality of the public Internet so that it can host backend software, transforming it into a global computing platform. Using the Internet Computer, developers can create websites, enterprise IT systems, and internet services by installing their code directly on the public Internet and dispensing with server computers and commercial cloud services.

[Website](https://internetcomputer.org/), [Medium](https://medium.com/dfinity)

**\[2\] Decentralized Finance**

Decentralized Finance (DeFi) is an open and global financial system built for the internet age — an alternative to a system that’s opaque, tightly controlled, and held together by decades-old infrastructure and processes. It gives you control and visibility over your money. It gives you exposure to global markets and alternatives to your local currency or banking options. DeFi products open up financial services to anyone with an internet connection and they’re largely owned and maintained by their users. So far tens of billions of dollars worth of crypto have flowed through DeFi applications and it’s growing every day.

[Website](https://ethereum.org/en/defi/)

**\[3\] Reverse Gas Modal**

Internet Computer uses a “reverse gas model”. Canisters pay for computation and ongoing persistence of memory using their own gas (called “cycles”).

[Website](https://twitter.com/dominic_w/status/1330996244190175232?lang=en)

**\[4\] Ethereum**

Ethereum is a decentralized, open-source blockchain with smart contract functionality. Ether (ETH or Ξ) is the native cryptocurrency of the platform. After Bitcoin, it is the largest cryptocurrency by market capitalization. Ethereum is the most actively used blockchain.

[Website](https://ethereum.org/en/), [Wikipedia](https://www.investopedia.com/terms/l/legal-tender.asp)

**\[5\] Aave**

Aave is an open-source and non-custodial liquidity protocol for earning interest on deposits and borrowing assets. It shifts from a decentralized P2P strategy to a pool-based strategy.

[Website](https://aave.com/), [Whitepaper](https://github.com/aave/protocol-v2/blob/master/aave-v2-whitepaper.pdf)

**\[6\] Gas Fee**

Gas fees are payments made by users to compensate for the computing energy required to process and validate transactions on the Ethereum blockchain.

[Investopedia](https://www.investopedia.com/terms/g/gas-ethereum.asp)

**\[7\] Chain Key Technology**

Chain Key Technology is a 48-byte public chain key rendering old blocks unnecessary which enables the Internet Computer to operate at web speed.

[Website](https://dfinity.org/faq/chain-key-technology)

**\[8\] Network Nervous System (NNS)**

The NNS is the autonomous software that governs the Internet Computer and manages everything from economics to network structure. The NNS is hosted within the network itself and is part of the system of protocols that securely weaves together the compute capacity of node machines to create the Internet Computer blockchain network, allowing the network to be autonomous and adaptive. The NNS acts as an autonomous “master” blockchain with a public key to validate all ICP transactions.

[Website](https://dfinity.org/faq/network-nervous-system-(nns))

**\[9\] Motoko**

Motoko is a programming language that is designed to seamlessly support the programming model of the Internet Computer, making it easier to efficiently build applications and take advantage of some of the more unique features of the platform. Motoko is strongly typed, actor-based, and has built-in support for orthogonal persistence and asynchronous message passing. Productivity and safety features include automatic memory management, generics, type inference, pattern matching, and both arbitrary- and fixed-precision arithmetic. Messaging transparently employs the Internet Computer’s Candid interface definition language and wire format for typed, high-level, and cross-language interoperability.

[Website](https://dfinity.org/technicals/motoko)

**\[10\] Type System**

In programming languages, a type system is a logical system comprising a set of rules that assigns a property called a type to the various constructs of a computer program, such as variables, expressions, functions, or modules. These types formalize and enforce the otherwise implicit categories the programmer uses for algebraic data types, data structures, or other components (e.g. “string”, “array of float”, “function returning boolean”).

[Wikipedia](https://en.wikipedia.org/wiki/Type_system)

Acknowledgments:
================

Interviewee: Dylan Paul, Malika Rawal

Interviewer: Xinyu Tian, Zesen Zhuang

Associate Editor: Zichao Chen

Executive Editors: Xinyu Tian, Zesen Zhuang

Chief Editor: Prof. Luyao Zhang
