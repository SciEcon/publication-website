Towards Incentivized Decentralization: The Future of Blockchain
===============================================================

**— Interview with Prof. Justin Cappos on decentralization, efficiency, and the ecosystem of blockchain**

About Prof. Justin Cappos
=========================

![](https://miro.medium.com/max/906/1*r0vSESXNq8x2juha4K8xUQ.png)<br />Figure  1: Prof. Justin Cuppos

[Justin Cappos](https://en.wikipedia.org/wiki/Justin_Cappos) is a professor in the Computer Science and Engineering department at New York University. Justin’s research philosophy focuses on improving real-world systems, often by addressing issues that arise in practical deployments.

![](https://miro.medium.com/max/1130/1*IxcPmXI5si2b_1t43KoDIA.png)[Figure 2: Stork](https://www2.cs.arizona.edu/stork/about.html)

His dissertation work was on [Stork](https://www2.cs.arizona.edu/stork/about.html), the first package manager designed for environments that use operating system virtualization, such as cloud computing. Improvements in Stork, particularly relating to security, have been widely adopted and are used on the majority of Linux systems via integrations into Apt, YUM, YaST, and Pacman. His later research advances have been adopted into production use including by [Microsoft, IBM, VMware, Cloudflare, Docker, RedHat](https://theupdateframework.com/), [ControlPlane, Datadog](https://in-toto.io/), and [git](https://www.usenix.org/system/files/conference/usenixsecurity16/sec16_paper_torres-arias.pdf), as well as a substantial percentage of automobiles. More information is available at [https://ssl.engineering.nyu.edu/personalpages/jcappos/](https://ssl.engineering.nyu.edu/personalpages/jcappos/).

![](https://miro.medium.com/max/1130/1*cCbKhUFe5gCvKrgWw_WWCw.png)<br />Figure  3: Companies that are using Prof. Cappos’s products

[Research Interests:](https://scholar.google.com/citations?user=COE6KUgAAAAJ&hl=zh-CN) Practical security, virtualization, cloud computing, software update systems, testbeds.

A Letter for Readers
====================

> Dear Readers:
> 
> I hope this letter finds you well! Here is the AMA (Ask Me Anything) team from SciEcon.
> 
> Blockchain provides new opportunities to our economy via decentralization. However, decentralization is only the means but not the ultimate goal. The current decentralized system often falls far behind its centralized counterparts in economic efficiency.
> 
> Prof. Justin Cappos is an expert in computer science. Abundant research of him improves real-world systems through technology. His research philosophy reflects an ancient Chinese saying, “being sageliness within and kingliness without, “ i.e., he observes the world rigorously with a grand vision and devotes himself passionately to the advances of humanity. He is a philosopher obsessed with the principle of the world, offering profound insights into Blockchain. He is a warrior at the forefront of academia, benefiting many big-named companies in the industry. He is a king who cares about the whole world, promoting Blockchain’s open-source and inclusiveness. He is also a poet imagining the future. Seattle that he creates empowers the splendid blueprint of P2P.
> 
> In the interview, Prof. Cappos talked about the vital role of Blockchain in the information and intelligence era. He addressed the dilemma between decentralization and economic efficiency. Then, he shared his optimistic view on content transmission and introduced his team’s latest achievements in improving computational and economic efficiency. Prof. Cappos took the Linux system as an example to illustrate his ambition in an open-source and inclusive blockchain system. Prof. Cappos also inquires DFINITY engineers about the contribution of Internet Computers to our current practice.
> 
> Now let’s see what insights we can get from Prof. Cappos.
> 
> Best wishes,
> 
> SciEcon AMA

Listen to the podcast on [Buzzsprout](https://www.buzzsprout.com/1801017/8780653-interview-for-prof-justin-cappos-english.mp3?download=true)

1\. What is your motivation for doing research about fintech/blockchain?
========================================================================

![](https://miro.medium.com/max/1130/1*In6D-9uSgZUXpmf-AC9PAw.png)[Figure 4: Centralized vs Decentralized vs Distributed Network: An Overview](https://blockchainengineer.com/centralized-vs-decentralized-vs-distributed-network/)

Prof. Cappos:
-------------

> **People around me care about blockchain**
> 
> I saw many people starting to talk about and work on different things related to blockchain and its potential. I specifically saw people doing resource-backed cryptocurrencies, things like [Filecoin](https://filecoin.io/) \[1\], and other things meant to provide some tangible good, or at least computational tangible good. I looked a lot about the systems and didn’t think they necessarily make a lot of sense.
> 
> **Centralization is more efficient than decentralization**
> 
> Because in general, if you have a good, like storage, memory, and computer power, that’s more efficient to centralize, then your system has this natural gravity where you end up with a lot of the mining power being centralized, which defeats a lot of purposes of having a decentralized system. For instance, the largest Bitcoin mining pools comprise scary amounts of computational power and could potentially do quite harmful things, specifically if a few of them collaborate.
> 
> **What good can a decentralized system bring to us?**
> 
> Once again, the problem is that they are not really that decentralized. And secondly, your incentives are pulling you toward centralization because centralized solutions usually are much more efficient than decentralized ones. I looked into this and thought would anything make sense in this space. That is how I get started and try to convince myself if anything would actually make sense here.

2\. Can you briefly highlight your research in the field of fintech/blockchain?
===============================================================================

![](https://miro.medium.com/max/926/1*S7MyDG2vrlial1xxCZbd6w.png)[Figure 5: Open Source Initiative](https://opensource.org/)

Prof. Cappos:
-------------

> **Content delivery is where we can make a change**
> 
> Specifically, I have an interest in resource-backed cryptocurrency. In general, fintech or other blockchain solutions make more sense than resource-backed ones tend to. I think they have a long way to go, and they have a whole set of problems. Resource-backed cryptocurrencies, for me, are something that I try to understand if I think there is something meaningful here because of the nature of the system.
> 
> Six years ago, I started to think about this problem fairly seriously. Since these resources, such as computer memory, bandwidth between nodes, storage, are more efficient for Google to provide in data centers, and home users try to get these, are there some resources that really need to be decentralized? The most promising one I could think of was content delivery, the [CDN networks](https://en.wikipedia.org/wiki/Content_delivery_networkv) \[2\]. CDN is basically when you want to watch movies, they are being retrieved from nodes very close to you rather than a server at the original company that actually has it. That is what makes Netflix and YouTube’s services faster because the videos are closer.
> 
> **We built an efficient decentralized system and commercialized it**
> 
> As I have targeted resources, the big problems were: Can you do this securely and efficiently? In terms of efficiency, I’m not just saying computational efficiency, but also economic efficiency. I spent four-plus years working with my Ph.D. students on a lot of these problems. To be honest, a bit to my surprise, we were able to build a system that is quite efficient and seems to have all the right economic and security properties and actually be successful in the marketplace.
> 
> And then, we founded a start-up, did a little bit of work there, and handed the technology over to the Linux Foundation. We have a bunch of folks working to commercialize it. We are working to make this something community-driven, in the spirit of open-source software and an open, mutually beneficial ecosystem where all participants can direct value that is not tightly controlled by only one company in this space.
> 
> **Modeling Linux, we try to make all participants equal in the ecosystem**
> 
> I have seen a lot of systems where for-profit companies or foundations make all the money. So, I also tried my best to make it more like an open-source project that meets an economic marketplace. Imagine something like a sporting league, where anyone can put a team together and compete and the league-provided umpires keep it fair. The umpires obviously have to be insulated from influence and you need a robust series of checks and balances. Fortunately, open-source projects and non-profit foundations when run correctly, have experience with handling these sorts of conflicts. Anyone who wants to come, and play is on equal footing with other people in the ecosystem. That’s really how you end up with the best ecosystem possible. The reason why Linux is the most successful operating system in the world has everything to do with the fact that anybody and everybody pitches in to fix issues despite the fact that Microsoft makes an enormous amount of money from the operating system and spent an enormous amount on it. I think Linux is really the success story and the thing we are trying to model.

3\. How do you think the Internet Computer can possibly empower your research? What support do you need to innovate with the Internet Computer? What technique questions do you have for the DFINITY engineers?
===============================================================================================================================================================================================================

![](https://miro.medium.com/max/1130/1*yZ9hT_1GRm1kQDKYfuyOYA.png)[Figure 6: DFINITY Internet Computer](https://medium.com/coinmonks/internet-computer-icp-biggest-launch-of-2021-467e19d33400)

Prof. Cappos:
-------------

> I think much of the Internet Computer’s introduction is for marketing pitch focus. In general, it’s not very clear what problems they are solving. Other than that, there don’t exist decentralized internet computers.
> 
> If I come to you and say I want to build a quantum computer because physics is cool and everybody likes physics, that might not be a good reason. But if we say we can crack all kinds of cryptographic codes, solve legitimate problems, and save billions of dollars a year by doing this, then you will be interested.
> 
> I am not sure what problems they are solving because running smart contracts isn’t the problem we have right now. Or maybe it’s a solution to a problem I don’t know.
> 
> My questions for DFINITY developers would be: In what domains are you solving problems? What problems are you solving over what’s currently being done? And how? Because now, I can go to Amazon’s [EC2](https://aws.amazon.com/ec2/?nc1=h_ls&ec2-whats-new.sort-by=item.additionalFields.postDateTime&ec2-whats-new.sort-order=desc) \[3\] and rent computing power. There are other systems to output like [EdgeNet](https://www.edge-net.org/), they provide computing to academic researchers. I built a peer-to-peer computing platform called [Seattle](https://seattle.poly.edu/) that ran for many years that provides that sort of computation. I’m not sure what real-world issues they are solving with their computational platform.

![](https://miro.medium.com/max/1130/1*l7IXUGmH1JzxGBxzbgzAZg.png)[Figure 7: Seattle : Open Peer-to-Peer Computing](https://seattle.poly.edu/)![](https://miro.medium.com/max/1130/1*FC77wu5ufRpsgWifGEDqCQ.png)[Figure 8: Logo of Edgenet](https://www.businesswire.com/news/home/20181029005591/en/Edgenet%E2%80%99s-New-Product-Experience-Management-Platform-Attracting-Record-Numbers-of-New-Users-in-Hardline-Industry)

Conclusion
==========

**Prof. Cappos’s questions for DFINITY engineers and developers:**

> 1\. We can already run smart contracts in the Ethereum blockchain. What specific advantages does the Internet Computer have over Ethereum in running smart contracts? How does the importance of DFINITY manifest in this space?
> 
> 2\. How does the Internet Computer ensure that it provides a truly decentralized system? What technologies help contribute to this landscape and how?
> 
> 3\. We can get computing services from Amazon EC2, EdgeNet, and other platforms. So, what’s new can DFINITY bring to issues about computations? How differently does the Internet Computer empower computing than the existing technologies?

Relevant Materials
==================

\[1\] Filecoin:

■ **_What is Filecoin?_**

Filecoin (⨎) is an open-source, public cryptocurrency and digital payment system intended to be a blockchain-based cooperative digital storage and data retrieval method.

■ **_What problems does Filecoin try to solve?_**

Unlike cloud-storage companies like Amazon Web Services or Cloudflare, which are prone to the problems of centralization, Filecoin leverages its decentralized nature to protect the integrity of a data’s location, making it easily retrievable and hard to censor.

[\[Website\]](https://filecoin.io/) [\[Wikipedia\]](https://en.wikipedia.org/wiki/Filecoin) [\[Slack\]](https://filecoin.io/slack) [\[Forum\]](https://github.com/filecoin-project/community#forums) [\[Github\]](https://github.com/filecoin-project) [\[WeChat\]](https://weixin.qq.com/r/1xz54Y-EctINrcuC90nF)

\[2\] CDN:

![](https://miro.medium.com/max/1130/1*S4fKXd6zuju8fEXMUs7aiQ.png)[Figure 9: Content Delivery Network](https://www.plesk.com/blog/tag/content-delivery-network/)

■ **_What is CDN?_**

CDN is abbreviated for a content delivery network or content distribution network. CDN is a geographically distributed network of proxy servers and their data centers. The goal is to provide high availability and performance by distributing the service spatially relative to end-users.

■ **_What good can CDN bring to us?_**

CDN nodes are usually deployed in multiple locations. Benefits include reducing bandwidth costs, improving page load times, or increasing the global availability of content.

■ **_How do CDN providers profit?_**

Traditionally, CDN providers profit either from direct fees paid by content providers using their network, or profit from the user analytics and tracking data collected as their scripts are being loaded onto customers’ websites inside their browser origin.

[\[Wikipedia\]](https://en.wikipedia.org/wiki/Content_delivery_network) [\[YouTube\]](https://www.youtube.com/watch?v=Bsq5cKkS33I)

\[3\] Amazon EC2:

![](https://miro.medium.com/max/1130/1*Jxx7cWrY21Sf9TFyodSZVA.png)[Figure 10: Amazon EC2](https://allcode.com/amazon-ec2/)

■ **_What is EC2?_**

Amazon Elastic Compute Cloud (EC2) is a part of Amazon.com’s cloud-computing platform, Amazon Web Services (AWS), that allows users to rent virtual computers on which to run their own computer applications.

■ **_What does Amazon say about EC2?_**

Amazon EC2 is a web service that provides secure, resizable compute capacity in the cloud. It is designed to make web-scale cloud computing easier for developers. Amazon EC2’s simple web service interface allows you to obtain and configure capacity with minimal friction. It provides you with complete control of your computing resources.

[\[Wikipedia\]](https://en.wikipedia.org/wiki/Amazon_Elastic_Compute_Cloud) [\[Website\]](https://aws.amazon.com/ec2/?nc1=h_ls&ec2-whats-new.sort-by=item.additionalFields.postDateTime&ec2-whats-new.sort-order=desc)

Acknowledgements
================

Interviewee: Prof. Justin Cappos

Interviewer: Prof. Luyao Zhang, Ray Zhu

Executive Editors: Xinyu Tian, Lunji Zhu

Chief Editor: Prof. Luyao Zhang
