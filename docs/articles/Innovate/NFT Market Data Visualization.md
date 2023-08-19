**NFT Market Data Visualization**
=================================================

**Disclaimer: This article is a final deliverable from Prof. Luyao Zhang’s project entitled “From ‘Code is Law’ to ‘Code and Law’: A Comparative Study on Blockchain Governance,” supported by the 2023 Summer Research Scholarship (SRS) program at Duke Kunshan University. Our Summer 2023 scholars also receive additional support from Wang-Cai Biochemistry Lab Donation Fund. SciEcon wholeheartedly supports DKU’s noble mission of advancing interdisciplinary research and fostering integrated talents. Our support is solely focused on promoting academic excellence and knowledge exchange. SciEcon does not seek any financial gains, property rights, or branding privileges from DKU. Moreover, individuals involved in this philanthropy event perform their roles independently at DKU and SciEcon.**

**Keywords**
#NFT #Classification # Blockchain #DataAnalysis #Algorithms #Data

Highlights:
Research: Use image analysis in the NFT and Blockchain space to extract meaningful features and develop an algorithm for automated image classification.
Innovation: Explore the NFT image space, and how machine learning and image recognition methodology can be applied to increase our understanding.
Leadership: Advance the scope of research on NFTs, and provide a comprehensive overview of the existing dataset availability/challenges.
GitHub Repository: https://github.com/SciEcon/SRS2023_NFT_Johnson

**Background**
================================

Non-Fungible Tokens (NFTs) have gained significant popularity in recent years as a new form of digital asset. NFTs are unique tokens that certify ownership using blockchain technology. This article will focus on analyzing a dataset drawn from the article ‘Mapping the NFT Revolution: market trends, trade networks, and visual features’ (Nadini et al., 2021). The dataset contains 6.1 million trades of 4.7 million distinct NFTs between June 23, 2017, and April 27, 2021. Ethereum blockchain data was scraped from four separate APIs: CryptoKitties sales, Gods-Unchained, Decentraland, and OpenSea. This means that data is broadly drawn from various areas of the NFT marketplace, and includes many different types of NFT. These NFTs are stored in a hand-classified linked dataset [1], in 6 distinct categories: Art, Collectible, Metaverse, Games, Utility, and Other. There are 1.2 million unique graphical images included in the linked dataset, meaning that in order to perform image analysis on the dataset redundancies will have to be removed (out of 6.1 million Excel rows, the dataset only contains 1.2 million unique graphical images). The complete dataset Excel file is too large to work with as a single unit, and so has been split into 79 distinct Pandas DataFrames, which have been preprocessed to remove certain redundancies. For ease of preliminary analysis, a random sample has been selected from each data frame, which has resulted in a reduced but statistically representative preliminary dataset to work with.

**Data Description and Cleaning Process**
================================

The queried data contains 24 columns. For certain token types, columns have ‘0’ values, but these have been incorrectly exported into the Pandas DataFrame, resulting in datatype errors. As part of the cleaning process, I have recorded these ‘Null’ values to not throw this error message. Every image has 4 columns with URL download links, where the NFT image can be downloaded. This is to ensure that the image is accessible even if it is deleted at the original download access point. The unique_id_collection column gives a unique token identifier for a given NFT. This unique identifier has been used to clean the dataset, and duplicate values/image URLs have been removed for processing. Two columns, Price_Crypto and Price_USD record transaction value with daily resolution, giving an accurate estimate of NFT valuation for every item in the dataset. There is also a Datetime column with the time of sale. This allows the tracking of NFT sales and market patterns both within a collection over time, or of an individual NFT id value over time. Data can also be sorted using the Market column, which displays the Market which data was downloaded from. These markets are unbalanced in the type of NFT which is predominant, and these have been visualized using a 3-dimensional bar chart. Finally, there is a Category column, listing which of the 6 categories a given image belongs to. This is highly important for conducting any type of image recognition analysis, as it allows the images to be correctly categorized, both to create a training dataset and verify the test dataset.

![](https://miro.medium.com/v2/resize:fit:1400/0*5B-ndUzSiAn4Ot6L)<br />Figure  1: Data Descriptors.

**Data Visualization and Preliminary Analysis**
================================

For data visualization and preliminary analysis, this article focuses on 5 variables: Price_USD, Datetime_Updated, Market, Category, and the scraped image datafile. The 6 categories of NFT are unevenly distributed across markets (fig. 2). Figure 2 shows that OpenSea has not only the largest overall number of NFTs but also the total highest number for each individual category. This emphasizes the importance of OpenSea in the NFT market, even while other more specialized markets have been queried which focus on specific types of NFT. Additionally, the average NFT price has been compared as filtered by category (fig. 3). Metaverse and utility tokens are traded at the highest average valuation, although this does not necessarily indicate that these token types dominate when it comes to market capitalization. In fact, it appears the case that Art, while 3rd in terms of average valuation, has the highest share of transactions, and a relatively high market capitalization (fig. 5) (Nadini et al., 2021). It is also important to look at the change in trading valuation over time (fig. 4). Examining both Metaverse and Art valuation, as well as collectibles, shows a trend across all 3 token types; a massive uptick in valuation beginning in late 2020 and resulting in market price fluctuation moving into 2023. Figure 4 draws attention to the correlation between different categories’ pricing, and especially to the recent explosion in NFT valuation and market capitalization.


![](https://miro.medium.com/v2/resize:fit:640/0*aJD90G2iVdWroHE8)<br />Figure  2: NFT category graphed against the market. Notice the relative dominance of OpenSea in terms of volume and the comparative frequencies of NFT types.

![](https://miro.medium.com/v2/resize:fit:720/0*IOkWVkPOlA_-wGrH)<br />Figure  3: Average price in USD filtered by category. Categories are Metaverse, Utility, Art, Collectible, Games, and Other. This visualization only includes queried data and is not a truly accurate or proportional representation of the overall NFT market. For example, because all NFTs in the ‘Gods Unchained’ ecosystem have been queried, this has shifted the reflected average price and is not representative of, say, the average price of ‘Gaming’ type NFTs on OpenSea.

![](https://miro.medium.com/v2/resize:fit:720/0*XPVhaKLNtKqr2gS0)<br />Figure  4: Average trading price in USD over time. Three similar categories, Metaverse, Art, and Collectible are simultaneously displayed.

![](https://miro.medium.com/v2/resize:fit:720/0*bfb7oXGl3BDvDUsr)<br />Figure  5: Data Descriptor (total trading volume). This graphic shows the relative (stacked) share of volume for given NFT categories. Note how Art, while not the highest by average valuation, does make up the majority of the trading volume.

**Conclusion & Discussion**
================================

It is important to highlight several limitations with both this and prior analysis of the same data. Despite querying an extensive dataset, it has currently only been used in broad strokes to provide an overview of the general NFT space. Therefore, the current research space does not sufficiently explore methods for feature extraction from images or machine learning for price prediction. This data has not been extensively applied to model pricing or to extract features from images. While it does appear that there are some more recent citations that investigate this idea, there remain promising unexplored directions for research in this vein.

Building upon insights gained from this data visualization project, future research can further employ image analysis techniques to extract meaningful features from NFT artwork in the workflow below:

Extract AI-created image descriptors from the set of NFT artwork images, and analyze these to describe visual characteristics.
develop a categorization algorithm that can automatically categorize images into one of the 6 predefined categories. This utilizes the dataset effectively and in a unique way, specifically capitalizing on the fact that it is a linked dataset, with image classifications already hand-assigned for every NFT. Several algorithms may be effectively applied for a comparative analysis of algorithm efficacy. These include Random Forest (combining multiple decision trees), K-Nearest Neighbor (KNN), and Deep Neural Network (training multiple layers). These research methods will help in understanding a- the nature of trading patterns in the NFT market and b- automatically classify existing NFTs and their associated images, using an AI-driven approach.
There are several research questions that are promising to explore. For instance: what trading patterns are visible in the NFT market, and how do trends differ across NFT categories and collections? What are the most effective image analysis techniques for capturing visual characteristics and assisting in automatic image classification/categorization? What image aspects are most important in predicting NFT valuation, and can a deep learning predictive model outperform a simple regression approach?

**About the Author**
================================

My name is Colden Johnson, I am a rising Sophomore student at Duke Kunshan University. I am considering a major in either Political Economy or Computation and Design with a track in Computer Science. My current research goals lie at the intersection of these two fields, and I am specifically interested in applying artificial intelligence and computation to address questions in the humanities.

**Acknowledgments**
================================

I am thankful to the following people for their helpful comments to improve this article, and especially to Prof. Luyao Zhang for her insightful feedback as my research mentor. I would also like to thank both Yiyang Zhang and Jiayi Wang for their feedback on this article.

Interim Executive Editors: Xintong Wu, Wanglin Deng, Yutong Quan

Associate Editor: Xinyu Tian

Chief Editor: Prof. Luyao Zhang

Design: Yixuan Li