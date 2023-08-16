NFT Marketplace Data Analysis
====================================================================================
Exploring trading trends and potential issues in the NFT marketplace
----------------------------------------------------------------------------------

> Disclaimer: This article is a final deliverable from Prof. Luyao Zhang’s project entitled “From ‘Code is Law’ to ‘Code and Law’: A Comparative Study on Blockchain Governance,” supported by the 2023 Summer Research Scholarship (SRS) program at Duke Kunshan University. Our Summer 2023 scholars also receive additional support from Wang-Cai Biochemistry Lab Donation Fund. SciEcon wholeheartedly supports DKU’s noble mission of advancing interdisciplinary research and fostering integrated talents. Our support is solely focused on promoting academic excellence and knowledge exchange. SciEcon does not seek any financial gains, property rights, or branding privileges from DKU. Moreover, individuals involved in this philanthropy event perform their roles independently at DKU and SciEcon.

**Keywords(hashtags)**
================

#NFT #DataAnalysis #account transparency #NFT event type

**Highlights:**
================

1.Research: This article conducts data analysis on NFT marketplaces, focusing on Ethereum and exploring trading trends, including changes in asset characteristics, transparency of transaction accounts, types of events, and distribution of asset links while raising further research questions.

2.Innovation: This article innovatively analyzes data sets from NFT marketplaces, providing insights into the evolving dynamics of the NFT ecosystem and raising important questions for further exploration.

3.Leadership: This article focuses on the exploration of NFT marketplace data analysis, leading the way in understanding trading trends and potential issues within the NFT ecosystem while providing valuable insights for further research and industry understanding.

**Supplementary Code**
================
https://github.com/SciEcon/SRS2023-NFT_Marketplaces

**Introduction**
================

The NFT marketplace provides a platform for NFT assets to be minted, traded, and other events. I had been conducting a comparative research study between permissioned blockchains and permissionless blockchains in the previous article entitled “[Deep dive on NFT marketplaces](https://medium.com/sciecon-research/deep-dive-on-nft-marketplaces-37c43162ab64)”, but I have encountered difficulties in obtaining sufficient datasets for permissioned blockchains. Most of the transaction data and other relevant information for permissioned blockchains, such as the notable examples of [Ali Antchain](https://antchain.antgroup.com/products/openchain) [1], are not openly accessible. As a result, the quality and quantity of available datasets for permissioned blockchains are insufficient, and the data obtained from secondary sources may have low credibility. Therefore, in this exploratory research article, I have decided to focus on studying datasets related to permissionless blockchains, specifically Ethereum. Ethereum stands out as one of the most renowned and widely used public blockchain platforms, providing abundant data available for research purposes.

By offering a comprehensive dataset on NFT marketplaces, [Understanding Security Issues in the NFT Ecosystem](https://arxiv.org/abs/2111.08893) [2] facilitates extensive analysis and research in the field (Das et al. 2021). The data relating to assets (such as collection names, asset URIs, metadata URIs, etc.) and events (such as minting, buying, selling, creating auctions, placing bids, accepting bids, transferring, etc.) are stored in the databases of the leading NFT marketplaces including OpenSea, Axie, CryptoPunks, Rarible, SuperRare, Sorare, Foundation, and Nifty. The dataset is categorized and collated by different NFT marketplaces and released as open access on GitHub: https://github.com/ucsb-seclab/nft-security-study. To facilitate further analysis, in the process of preliminary processing, the main data of different NFT marketplace data sets are retained according to relevant keywords, and the files occupying smaller storage media are re-generated to improve the efficiency of data processing.


**Data Information and Preprocessing**
================
![](https://miro.medium.com/v2/resize:fit:1400/format:webp/1*5FSjtAlzEP1ppxr7MGG0hg.jpeg)<br />Figure 1: Description of citing Raw Database.

The data analysis in this article relies on the database from [Understanding Security Issues in the NFT Ecosystem](https://arxiv.org/abs/2111.08893), which comprises 10 folders containing data on various aspects of the NFT ecosystem. However, a critical limitation of using this database lies in the potential lack of credibility and reproducibility of secondary studies that rely on non-primary data sources. Since the primary data collection process is not explicitly documented, it becomes challenging for interdisciplinary researchers to verify or replicate the findings independently. Without transparent access to the primary data sources, the risk of introducing biases or errors in the analysis increases, undermining the overall credibility of the research. Moreover, the lack of detailed information on data collection methodologies and potential data biases may further hinder the reproducibility of results, impeding the advancement of knowledge in the field.

![](https://miro.medium.com/v2/resize:fit:1400/format:webp/1*JkNQ8qm4XwdvsUbAYl-JlA.jpeg)<br />Figure 2: Raw Database Information Available to me (Created based on the data source content).

Initially, the extracted dataset posed a significant challenge for analysis, as it exceeded 300GB in size. Some of these folders contained files larger than the typical operating memory of a regular laptop, making it difficult to work with the data directly. Moreover, the suggested basic approach to handle this dataset was using PostgreSQL. However, as an undergraduate student lacking previous experience in PostgreSQL skills, I opted to directly unzip the files and read the data using Microsoft Office tools. This reliance on specific data processing skills could hinder the wider dissemination and application of this dataset to a broader audience. Moreover, a detailed data dictionary, if provided, would help me navigate useful meta data information such as column headers and the format of individual data points, from each list. Furthermore, each list in the dataset covered a slightly different time range, which could lead to noticeable discrepancies when plotting charts. Many elements in the data were represented by alphanumeric strings, such as Timestamps and transaction Hashes, and having a Data Dictionary or other detailed explanations of the data would have facilitated a better understanding of it.

![](https://miro.medium.com/v2/resize:fit:1400/format:webp/1*kNj86EE0wM0tiPmnxtcAbA.jpeg)<br />Figure 3: Data query process example.

During the data processing and analysis, I conducted a preliminary examination of the dataset and chose a limited number of variables that were deemed relevant. Other data considered less relevant was intentionally omitted. By utilizing keyword extraction techniques, the size of the dataset was significantly reduced. Consequently, a CSV file was generated containing only the selected columns, making it easier for further processing and analysis. Notably, in the context of account accessibility, I added an extra column indicating the presence of account information in the original data and used binary values (0 and 1) to measure accessibility. This approach allowed for the creation of a more manageable dataset tailored to a specific investigative focus. It is essential to recognize that this approach, while pragmatic, may result in the loss of potentially valuable insights or correlations that could be inherent in the omitted variables.

![](https://miro.medium.com/v2/resize:fit:1400/format:webp/1*aAeePzbqJI8ur7BsV--4dg.png)<br />Figure 4: Data Information (created on GitHub).

These files contain processed data related to NFT transactions and events on several NFT marketplaces. They provide information such as the size, duration, file type, and last transaction time of NFT assets on Foundation, accessibility of user names and addresses for both sides of the transaction on SuperRare and Rarible, classification of NFT events (such as minting, buying, selling, and auction creation) and their timestamps on Foundation, SuperRare, and Rarible, as well as image URLs of NFT assets on Nifty.


**Data Visualization and Analysis**
================
**The size, duration, file type, and last transaction time of NFT assets on the NFT market place: Foundation**

![](https://miro.medium.com/v2/resize:fit:1400/0*0m2PBN_hGa08Ihkg)<br />Figure 3: MIME Type Distribution on Foundation.

With the passage of transaction time, the proportion of video NFT in mp4 format gradually decreased from more than 50% to less than 50%. The NFT of the image type has gradually become the dominant file type, and the jpeg format continues to be the dominant image format. Worth noting is that post-August 2021, NFT file types have exhibited diversification, particularly with a noticeable increase in model categories. Additionally, various other file formats have been incorporated.

The possible reason for the decrease in video NFTs and the rise of image NFTs, particularly in jpeg format, could be attributed to a shift in user preferences towards static visuals for ease of access and display, and the future trend might indicate continued diversification with an increasing focus on 3D models and other file formats to cater to evolving demands and applications within the NFT market.

![](https://miro.medium.com/v2/resize:fit:1400/0*vosdsH_ulndtXsm5)<br />Figure 4: Average Width Variation of Video.

![](https://miro.medium.com/v2/resize:fit:1400/0*9bQmFYz08H71ggJq)<br />Figure 5: Average Height Variation of Video.

![](https://miro.medium.com/v2/resize:fit:1400/0*N-dopbSfA4zdtw4r)<br />Figure 6: Average Duration Variation of Video.

With the passage of trading time, the height and width of the NFT of the video type have gradually fluctuated from large to around 1700 pixels and 1500 pixels on average. Except for a few occasional super-long videos, the average length of the videos remained stable at less than a minute.

The possible reason for the fluctuation in height and width of video NFTs and the stable average length, except for occasional super-long videos, could be attributed to users’ preference for higher resolution and shorter, more digestible content, and the future trend might indicate a continuation of the pattern, with an increasing emphasis on optimized video formats for enhanced viewing experiences and wider accessibility.

![](https://miro.medium.com/v2/resize:fit:1400/0*eGF9lht8WmrpA0RB)<br />Figure 7: Average Width Variation of Image.

![](https://miro.medium.com/v2/resize:fit:1400/0*In3_tGCixeMfaEH2)<br />Figure 8: Average Height Variation of Image.

![](https://miro.medium.com/v2/resize:fit:1400/0*92V2seW-GWNLPWPP)<br />Figure 9: Average Height Variation of Image (Log Transformed).

With the passage of trading time, the width of the NFT of the image type gradually changes from a large fluctuation to a small fluctuation. Similarly, in the field of pictures, there are occasional oversized works. Given the less apparent changes in the smaller data, I opted for log transformation to facilitate further processing. The chart following the log conversion clearly illustrates how the height of image-type NFTs shifts from significant fluctuations to more subtle variations.

The possible reason for the transition from large to small fluctuations in the width and height of image NFTs, along with occasional oversized works, could be due to a growing understanding of optimal image dimensions and sizes among creators, resulting in more standardized and optimized image submissions, and the future trend might indicate a continued refinement of image specifications as creators prioritize consistency and user-friendliness in the NFT market.

**Inclusion Criteria**

![](https://miro.medium.com/v2/resize:fit:1134/0*cTHcXILHoaxAmKhW)<br />Figure 10: Account Accessibility of Transactions on Rarible.

![](https://miro.medium.com/v2/resize:fit:1134/0*A7n7-ePfgOhqy6hi)<br />Figure 11: Account Accessibility of Transactions on SuperRare.

In terms of the availability of accounts on both sides of the NFT transaction, the account addresses of both Rarible and SuperRare are searchable according to the existing database. In terms of account user name, both Rarible and SuperRare pay attention to the transparency of sender account user name in transactions, most sender account user name is searchable. In the recipient account, most user names are not searchable. The difference between the accessibility of the two accounts’ usernames is more obvious on SuperRare.

The possible reason for the difference in accessibility of account usernames between Rarible and SuperRare could be attributed to variations in their platform policies and user privacy settings, and the future trend might indicate a potential focus on enhancing user control over username visibility and transparency in NFT transactions to strike a balance between privacy and user engagement.


**Classification of NFT events on Foundation, SuperRare, and Rarible**

![](https://miro.medium.com/v2/resize:fit:1400/0*B1hPCDvkLyL_-XZ6)<br />Figure 12: Foundation Event Type.

Over time, list, mint, and bid continue to be the main NFT event types on Foundation. After February 2021, the types of NFT events have also diversified. PriceChange, Settle, and Sold also account for a portion of this. The total share of PriceChange and bid, and other types of events that can lead to market bubbles in NFT, has remained high.

The possible reason for the continued dominance of list, mint, and bid events on Foundation, along with the diversification of NFT event types after February 2021, including PriceChange, Settle, and Sold events, with a sustained high share of PriceChange and bid events, might be attributed to the growing interest and speculative nature of the NFT market, and the future trend might indicate a need for increased regulatory measures and market stabilization efforts to mitigate potential market bubbles in the NFT space.

![](https://miro.medium.com/v2/resize:fit:1400/0*13KsKH_pLyEEG8CG)<br />Figure 13: Rarible Event Type.

On Rarible, transfer, mint, and buy were the main types of early NFT events as they occurred over time. After June 2020, the types of NFT events have also diversified. After October 2020, the proportion of order events increased dramatically, becoming the most dominant NFT event. Other events such as offers also squeeze the proportion of NFT events such as transfer, mint, and buy.

The possible reason for the diversification of NFT events on Rarible, with a significant increase in order events after October 2020, becoming the most dominant event type, and other events like offer affecting the proportions of transfer, mint, and buy events, might be attributed to the platform’s evolving functionalities, increased trading activity, and the emergence of new features to cater to user demands, and the future trend might indicate a continued focus on order-based transactions and enhanced trading capabilities to accommodate the growing NFT market and user preferences.

![](https://miro.medium.com/v2/resize:fit:1400/0*EVQDcRSGh0cAxTMn)<br />Figure 14: SuperRare Event Type.

On SuperRare, the proportion of early major NFT event types has no specific law, which reflects the chaos of the NFT marketplace in the early stage. Over time, the bid event type gradually occupied the main position, but the subsequent proportion also gradually declined. After November 2020, the types of NFT events also showed a more significant diversity. The total share of the types of events that can lead to market bubbles, such as bids and sale price sets, has remained high.

The possible reason for the lack of specific patterns in early major NFT event types on SuperRare, followed by the gradual dominance and subsequent decline of bid events, and the increasing diversity of NFT events after November 2020, with a sustained high share of events that can lead to market bubbles, might be attributed to the NFT market’s early experimental phase and subsequent maturation, and the future trend might indicate a continued focus on mitigating market bubble risks through improved pricing mechanisms and regulatory measures to ensure a more stable NFT marketplace.


**Image URL types of NFT on Nifty**

![](https://miro.medium.com/v2/resize:fit:1400/0*EZFNQ0zx5QAJ5EiC)<br />Figure 15: Nifty Website Proportions.

A large proportion of the image capture links are stored on Nifty’s website, but there are also cases where image capture links are stored on other websites. There are also some specific periods in which the proportion of links to other websites has increased significantly, which may increase the risk of link failure. But after October 2020, the share of Nifty’s sites remained high.

The possible reason for the significant proportion of image capture links being stored on Nifty’s website, with occasional increases in links stored on other websites during specific periods, followed by a decline in such occurrences after October 2020, might be attributed to Nifty’s efforts to enhance platform stability and reduce the risk of link failures, and the future trend might indicate a continued focus on maintaining a robust and reliable image storage infrastructure on Nifty’s website to ensure a seamless user experience and mitigate potential link-related issues.

To address the time range limitations of using an existing dataset for image generation, attempts have been made to obtain additional image capture links through Nifty’s API, leveraging keywords and other information. However, this method fails to ensure data randomness, and the newly acquired dataset remains considerably smaller compared to the original dataset. Furthermore, analyzing the proportion of image links from other marketplaces by using the existing dataset does not reveal other notable preferences for specific websites, hindering the demonstration of the overall universality of image storage security.

In addition, in [Understanding Security Issues in the NFT Ecosystem](https://arxiv.org/abs/2111.08893), Das et al. (2021) conduct an analysis of image storage security through URL address connectivity. Replicating a similar URL address analysis code for this article is impractical due to its computationally intensive nature, requiring several days to run and imposing a significant burden on the research. Therefore, I have not explored the potential for further research on Image URL security at present.



**Conclusion & Discussion**
============
In this exploratory research article, our focus was on analyzing datasets related to permissionless blockchains, specifically Ethereum, as obtaining sufficient datasets for permissioned blockchains posed difficulties. We conducted data visualization and analysis on various aspects of NFT transactions and events, shedding light on changes in NFT asset characteristics, transparency of NFT transaction accounts, shifts in NFT event types, and alterations in the type of access link for NFT assets. However, it is crucial to acknowledge the limitations of our data analysis. The data analysis primarily relied on data from Foundation, Rarible, SuperRare, and Nifty, which might have different mechanisms, especially in classifying NFT events.

Based on the previous research on sentiment analysis of CryptoPunks-related tweets and market changes of CryptoPunks before and after 2021, there are indeed some interesting directions for further exploration ([Zhang et al. 2023](https://arxiv.org/pdf/2307.10201.pdf)). One potential avenue is expanding the sentiment analysis to encompass various NFT marketplaces beyond CryptoPunks, which could provide valuable insights into user preferences and perceptions of different platforms in the NFT space. However, we must acknowledge limitations due to the non-availability of complete open-source Twitter data, which may hinder integrating NFTs and social media in future research.

Furthermore, NFTs’ popularity and profitability as a means of purchasing digital assets like art and music have resulted in significant sales, surpassing $25 billion in 2021. However, the lack of familiarity with NFT technology and the prevalence of scams on social media has led to fraudulent schemes targeting unsuspecting users ([Roy et al. 2023](https://arxiv.org/abs/2301.09806)). Based on our preliminary data analysis, several research questions can be explored to further understand the dynamics of the NFT ecosystem: How have the file types and formats of NFT assets evolved across different marketplaces? How transparent are the sender and recipient account usernames in NFT transactions across various marketplaces, and are there any privacy and safety concerns associated with the accessibility of account information? How are the types of NFT events evolving, and are there specific events becoming prominent that could add to the NFT marketplace bubble?

Considering the large size of the database drawn from multiple NFT marketplaces, the data analysis and raw data can also be leveraged for training Large Language Models (LLMs) to increase the likelihood of predicting NFT marketplace behavior.


**Relevant Materials**
============

[1] Ali Antchain

Ali Antchain (阿里蚂蚁链) is a consortium blockchain service network specifically designed for enterprises and developers. The streamlined approach to blockchain implementation eliminates the need for constructing a separate blockchain. Ali Antchain utilizes a fuel pricing mechanism similar to public chains, enabling users to enjoy cost-effectiveness and accessibility through features such as a fast deployment platform, various contract development templates, and flexible pricing options.

[[Ali Antchain](https://antchain.antgroup.com/products/openchain)]

[2] Linked Data

The dataset used in the ACM CCS 2022 paper titled “Understanding Security Issues in the NFT Ecosystem” includes asset and event data from the top 8 NFT marketplaces, historical prices of crypto coins from CoinGecko, and information on the availability of token contract source code in Etherscan. The asset and event data cover various aspects of NFT transactions and events, providing insights into the NFT ecosystem, while the additional data on crypto coins and token contracts contribute to understanding the broader context and security aspects of the ecosystem ([Das et al. 2021](https://arxiv.org/abs/2111.08893)).

[[Understanding Security Issues in the NFT Ecosystem](https://zenodo.org/record/6526192)]



**About the Author**
================
**Yiyang Zhang**

![](https://miro.medium.com/v2/resize:fit:1400/0*5lLxrxjsgCobC3B5)<br />Figure 11: Yiyang Zhang

*Yiyang Zhang* is from the class of 2025, majoring in Computation and Design with tracks in Digital Media at Duke Kunshan University. She is designated a Summer Research Scholar for the summer of 2023 and awarded by the SRS program. Her research interest is NFT transaction, digital design, and media interaction.

**Acknowledgments**
================

**Interim Executive Editors**: Xintong Wu, Wanlin Deng

**Associate Editor**: Xinyu Tian

**Chief Editor**: Prof. Luyao Zhang

**Design**: Yixuan Li

Thanks to Yutong Quan, Colden Johnson, and Jiayi Wang for peer review.
