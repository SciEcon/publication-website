**NFT Marketplace: Introduction to NFT and NFT marketplace’s mechanism**
========================================================================

**Introduction**
================

After many years of rapid growth in the blockchain industry, NFTs began to rise rapidly at the beginning of this year. As Dean Sam, a writer in Los Angeles Times, defined, non-fungible token (NFT) is a unit of data stored on the Blockchain that certifies a digital asset to be unique. NFTs can be used to represent digital files, such as photos, videos, audio, and so on. Moreover, the Blockchain will record the ownership and specific information about this asset. NFT is different from traditional physical goods, and they need new marketplaces. Many market platforms for trading NFT assets have been born on the Blockchain. With the rising price of NFT assets, more and more players have entered this field.

On March 11th this year, an NFT artwork named “Everydays — The First 5000 Days” was sold for an extremely high price of $69 million on Christie’s auction website, which shocked everyone [\[1\]](https://www.nytimes.com/2021/03/11/arts/design/nft-auction-christies-beeple.html). In addition, a lot of well-known companies are targeting the NFT market. In July, Coca-Cola, the world-famous beverage company, announced that it began selling its NFT souvenirs collection. Budweiser, another beverage giant, also began to buy NFT products in July. In the same month, Rolling Stone magazine has also joined the NFT market [\[2\]](https://www.forbes.com/sites/martyswant/2021/07/28/as-coca-cola-auctions-its-first-nft-more-brands-are-entering-the-metaverse/?sh=6573224a1051). Such examples have appeared a lot recently.

On the whole, the market is in a stage of rapid development. The whole NFT market achieved more than $2 billion in transactions in the first quarter of 2021 — which is 2000 percent higher than the fourth quarter of 2020 [\[3\]](https://www.cnbc.com/2021/04/13/nft-sales-top-2-billion-in-first-quarter-with-interest-from-newcomers.html). When seeing this shocking data, you may have doubts: Why can such virtual items sell at these extremely high prices? What are the prevailing technical standards? What are the mechanisms of the NFT auction? What does the NFT marketplace bring us? We prepared two NFT Marketplace articles for you. In this first article, I’ll introduce the questions above to you. And in the second article, we will instruct you on choosing the most suitable NFT marketplace for you.

![](https://miro.medium.com/max/1200/0*RJ4-DEGfIE7IN6yJ)<br />Figure  1: [“Everydays — The First 5000 Days” is a collage of all the images that the artist known as Beeple has been posting online each day since 2007.](https://www.nytimes.com/2021/03/11/arts/design/nft-auction-christies-beeple.html)

**Why can NFTs sell at such a high price?**
===========================================

For all goods, scarcity is a critical price determinant. At present, most of the goods in the NFT auction market are limited edition works of art, which have set a foundation for their price. In addition, NFT has a feature that traditional works of art cannot have, that is — — the display function in the information age. Just as the co-founder of CryptoPunks, John Watkinson, said, “there was a showing-off factor, flashing what you have to other people in a virtual way was the only way to do it.” [\[1\]](https://www.nytimes.com/2021/03/11/arts/design/nft-auction-christies-beeple.html) As the boss of the blockchain market, he is very familiar with the leading customer groups in the NFT market. “There are some wealthy individuals in Silicon Valley collecting these now. If you own a rare one of these, it’s meaningful,” he said. Just imagine, if you are a person who likes collecting artworks, you have a lot of great art at home. However, most of the time you can only enjoy them at home by yourself, or sometimes invite friends to visit at home. But now, you can buy NFT artworks, display them on all your social media platforms, and all Internet users can see that you own them on your home page. Are these feelings and experiences very attractive? In addition, NFT also has the characteristics of Blockchain. Others can see your ownership of these NFTs on the Blockchain. The above paragraphs explain why virtual collections can have such high value.

![](https://miro.medium.com/max/1020/0*F_YHeaBJ8kHtKfT4)[Figure 2: An NFT product from Coca Cola — bubble jacket.](https://www.nytimes.com/2021/03/11/arts/design/nft-auction-christies-beeple.html)

**The Technical Standards of NFT**
==================================

After discussing the formation of the NFT value, we should also understand the operation mechanism behind it. Therefore, the following content will be more in-depth and introduce the technical standards and characteristics. As a new blockchain product, NFT has many technical standards.

Different technical standards correspond to various methods of generating NFT on Blockchain. Commonly used token standards include [ERC-721, ERC-1155 and ERC-998](https://hackernoon.com/non-fungible-token-nft-standards-an-overview-w71y34y3) [\[4\]](https://hackernoon.com/non-fungible-token-nft-standards-an-overview-w71y34y3). Among them, ERC-721 is the most basic and popular one, ERC-1155 is the mainstream standard in the game industry, and ERC-998 can contain multiple tokens. The NFT marketplace developers may choose different standards. For example, OpenSea, one of the most popular NFT marketplace, only supports NFTs built with ERC-721 and ERC-1155 standards.

The most commonly used one among all is ERC-721. The first project that used ERC-721 is CryptoKitties, a collectible game that caused congestion on the Ethereum network in 2017 [\[5\]](https://blockonomi.com/cryptokitties/). And the standard ERC-721 was created and released by the project’s CTO, Dieter Shirley [\[6\]](https://tokenpocket-gm.medium.com/tpcourses24-history-of-nft-origin-b16b9ca0e036). Since then, ERC-721 has entered people’s vision. And it has become the most widely used NFT standard.

The second popular standard is ERC-1155. It is originated from game development. Enjin’s CTO, Witek Radomski, created ERC-1155 standard [\[7\]](https://enjin.io/help/erc-1155-ethereum-token-standard) . This standard was created for the reason that the game developers need to send props to multiple accounts in the game. However, it is costly to call a smart contract every time for each account. Thus, the ERC-1155 standard was created. Since it has both the characteristics of NFT and FT (Fungible Token), ERC-1155 is a so-called semi-fungible token. The main difference with NFT is that one token no longer refers to a specific item but a class of items. In other words, there is no difference between objects with the same token ID.

Another standard, ERC-998, is not as common as the above two standards, which establishes composable non-homogeneous tokens (CNFT) , whose structural design allows any NFT to be bundled with other NFTs or FTs [\[8\]](https://medium.com/arianee/an-exploratory-look-into-erc-998-composable-tokens-a057cd4f8c1a) . ERC-998 tokens can contain multiple ERC-721 and ERC-20 tokens. When transferring CNFT, it means moving the entire hierarchical structure and relationships of the CNFT. For example, in CryptoKitties, a cat can have non-fungible tokens, like a chain around the neck. ERC-998 can pack everything in one for transfer.

![](https://miro.medium.com/max/1400/0*EIvSbMbjjNsXyJMq)<br />Figure  3: [How Smart Contracts Works](https://2muchcoffee.com/blog/how-to-build-an-opensea-like-nft-marketplace/)

**What does the NFT Marketplace Bring Us?**
===========================================

When people create NFTs, they will naturally consider trading NFTs. Followed by many NFT trading markets, so what are their characteristics? The idea of digital trading assets in the NFT marketplace provides some unique advantages for creators and people like collectors and art enthusiasts. Taking digital artwork as an example, NFT has the potential to solve some of the shortcomings in the traditional art market. First, in the conventional art market, the fluidity of artwork is very poor. That is, a piece of artwork usually only changes its ownership a few times. However, trading artwork will become extremely easy via NFT marketplaces. Second, it is almost impossible for artists to get paid from the **second sale** of their artwork in the traditional art market. In contrast, many NFT marketplaces support artists to choose the percentage of royalties they want from secondary sales.

![](https://miro.medium.com/max/1400/0*tSB2pSdHKSUmLgMF)[Figure 4: Total number of sales involving a non-fungible token (NFT) in the art sector worldwide over the previous 30 days from April 12 to October 15, 2021, by type](https://www.statista.com/statistics/1235228/nft-art-monthly-sales-volume/)

Therefore, NFT marketplaces ensure users can browse and trade NFTs flexibly and solve the problems of creators’ income in the traditional market. Although all NFT marketplaces operate similarly, a hub dedicated to NFT transactions built on the Blockchain, different NFT marketplaces provide various functions.

![](https://miro.medium.com/max/1400/0*iZSGcFn9Z_-OST5H)<br />Figure  5: [NFT Marketplace System](https://semidotinfotech.com/blog/cost-to-develop-an-nft-marketplace/)

**The two mechanisms of NFT auction**
=====================================

Among all the NFT trading modes in the marketplace, the auction is the most popular and mainstream trading form. Many high-priced NFTs in the news were sold by auctions. When talking about NFT auctions on the network platform, it is unfamiliar to many people. In the public’s impression, the traditional auction is generally in a banquet hall, and the host stands on the stage shouting the current price. However, the auction of NFT is on the network trading platform. And there are two main auction mechanisms: centralization and decentralization.

![](https://miro.medium.com/max/1400/0*j1Orvk2LyXhvQDVK)[Figure6 Popular NFT Marketplaces](https://blog.gilded.finance/best-nft-marketplace/)

A decentralized NFT auction platform connects buyers to sellers via a smart contract. The smart contract handles the logic and transferring information between the bid of the NFT. This entire exchange happens fully on-chain. Many famous auction platforms are using this mechanism, including [OpenSea](https://opensea.io/), [Nifty Gateway](https://niftygateway.com/), etc. In the following, I will explain the advantages of the decentralized auction over the centralized auction. After that, you can also find the advantages of the decentralized auction. These two auction methods have their own advantages.

> The advantages of the decentralized auction:
> 
> 1\. Every bid is public and permanently recorded, which makes bids more secure and transparent.
> 
> 2\. It does not need a third-party agent; smart contracts will run the auction.

A centralized NFT auction platform has just emerged in recent months. This auction mechanism is off-chain bidding, which is similar to the traditional goods auction platform. It brings some advantages of centralization into the NFT auction platform. Artists and NFT sellers can still sell and buy NFT artworks on the platform, and the auction platform will send the works to the buyer’s wallet after the transaction.

> The advantages of the centralized auction:
> 
> 1\. Bidders can use fiat currency like US dollars. It is more convenient than buying cryptocurrency before an auction. Bidders don’t need to observe the price change of ETH, one of the most mainstream cryptocurrencies in the world, when bidding.
> 
> 2\. There is no need to pay gas fees when bidding, which is cheaper.
> 
> 3\. It provides a varied group of potential customers and helps the auction agent ensure the legitimacy of auction guests.
> 
> 4\. Customers can go back after taking the goods, although they have to pay a deposit.

According to the advantages of both decentralized and centralized auction provided above, we want to deliver the following suggestions to help you choose from the two auction mechanisms. First, if you are a new player in the NFT market and want to have your first try, the centralized auction is suitable for you. Because you don’t need to pay expensive gas fees when bidding. And you don’t need to create a crypto wallet, which means you can use fiat currency conveniently. Then, if you are an experienced NFT buyer or blockchain enthusiast, we recommend that you directly choose the decentralized auction. Because decentralized auction markets usually have more collectibles to choose from. In addition, decentralized auctions are more stable and faster.

In the end, we wish you to have a great buying experience, whether you’re a beginner or a veteran gamer. In the next article in this series, we will bring you a guideline and instructions for the selection of the NFT marketplace.

![](https://miro.medium.com/max/1400/0*OtARNbVCUhAJ4Ros)<br />Figure 7 Advantage of Each Auction Mechanism (created by Whimsical)

**Relevant Materials**
======================

**\[1\] ERC-721, ERC-1155 and ERC-998**

ERC-721 is the most basic and popular one, ERC-1155 is the mainstream standard in the game industry, and ERC-998 can contain multiple tokens.

[**\[Hackernoon\]**](https://hackernoon.com/non-fungible-token-nft-standards-an-overview-w71y34y3)

**\[2\] Dieter Shirley**

Dieter Shirley, Co-creator of CryptoKitties and ERC-721. Co-founder of Dapper Labs, Lead Architect of Flow. He is co-creator of CryptoKitties, the first mainstream blockchain experience outside of cryptocurrencies. Currently tackling the many technological barriers that are keeping the benefits of decentralization away from billions of citizens of the internet.

[**\[CypherHunter\]**](https://www.cypherhunter.com/en/p/dieter-shirley/)

**\[3\] Witek Radomski**

Witek Radomski is co-founder and CTO of Enjin, a leading NFT ecosystem developer. Witek wrote the code for one of the first-ever NFTs in 2017 and is the author of ERC-1155, the advanced Ethereum token standard that enables developers to deploy both fungible and non-fungible items in a single smart contract.

[**\[NonfungibleTokyo\]**](https://nonfungible.tokyo/speakers/witek-radomski/)

**References**

**\[1\] JPG File Sells for $69 Million, as ‘NFT Mania’ Gathers Pace — The New York Times**

[https://www.nytimes.com/2021/03/11/arts/design/nft-auction-christies-beeple.html](https://www.nytimes.com/2021/03/11/arts/design/nft-auction-christies-beeple.html)

**\[2\] As Coca-Cola Auctions Its First NFT, More Brands Are Entering The Metaverse — Fobes**

[https://www.forbes.com/sites/martyswant/2021/07/28/as-coca-cola-auctions-its-first-nft-more-brands-are-entering-the-metaverse/?sh=6573224a1051](https://www.forbes.com/sites/martyswant/2021/07/28/as-coca-cola-auctions-its-first-nft-more-brands-are-entering-the-metaverse/?sh=6573224a1051)

**\[3\] NFT sales top $2 billion in first quarter, with twice as many buyers as sellers — CNBC**

[https://www.cnbc.com/2021/04/13/nft-sales-top-2-billion-in-first-quarter-with-interest-from-newcomers.html](https://www.cnbc.com/2021/04/13/nft-sales-top-2-billion-in-first-quarter-with-interest-from-newcomers.html)

**\[4\] Non Fungible Token (NFT) Standards: An Overview — Hackernoon**

[https://hackernoon.com/non-fungible-token-nft-standards-an-overview-w71y34y3](https://hackernoon.com/non-fungible-token-nft-standards-an-overview-w71y34y3)

**\[5\] CryptoKitties: The Latest Excitement Sweeping the Ethereum Community — Blockonomi**

[https://blockonomi.com/cryptokitties/](https://blockonomi.com/cryptokitties/)

**\[6\] TPCourses24 — History Of NFT Origin — Medium**

[https://tokenpocket-gm.medium.com/tpcourses24-history-of-nft-origin-b16b9ca0e036](https://tokenpocket-gm.medium.com/tpcourses24-history-of-nft-origin-b16b9ca0e036)

**\[7\] ERC-1155 Ethereum Token Standard — Enjin**

[https://enjin.io/help/erc-1155-ethereum-token-standard](https://enjin.io/help/erc-1155-ethereum-token-standard)

**\[8\] Composable Tokens: How ERC-998 Works — Medium**

[https://medium.com/arianee/an-exploratory-look-into-erc-998-composable-tokens-a057cd4f8c1a](https://medium.com/arianee/an-exploratory-look-into-erc-998-composable-tokens-a057cd4f8c1a)

**\[9\] Art explained: How do art auctions really work? — CNN Style**

[https://www.cnn.com/style/article/how-do-art-auctions-work-steven-murphy/index.html](https://www.cnn.com/style/article/how-do-art-auctions-work-steven-murphy/index.html)

**\[10\] The Advantages of Buying Art at Auction — Artsy**

[https://www.artsy.net/article/artsy-specialist-advantages-buying-art-auction](https://www.artsy.net/article/artsy-specialist-advantages-buying-art-auction)

**\[11\] NFT Auction Platforms**

[https://medium.com/community-economics-by-forte/nft-auction-platforms-81d92f342604](https://medium.com/community-economics-by-forte/nft-auction-platforms-81d92f342604)

Author: Zichao Chen & Yufan Zhang, Duke Kunshan University
----------------------------------------------------------

**Project Instructor: Prof. Luyao Zhang**
-----------------------------------------

Acknowledgments:
================

Design: Austen Li

Executive Editors: Xinyu Tian

Chief Editor: Prof. Luyao Zhang
