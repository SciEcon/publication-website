Dynamics of Centralized and Decentralized Cryptocurrency Exchanges
====================================================================================

Analyzing ETH Token Trading on Centralized and Decentralized Cryptocurrency Exchanges
----------------------------------------------------------------------------------

> Disclaimer: This article is a final deliverable from Prof. Luyao Zhang’s project entitled “From ‘Code is Law’ to ‘Code and Law’: A Comparative Study on Blockchain Governance,” supported by the 2023 Summer Research Scholarship (SRS) program at Duke Kunshan University. Our Summer 2023 scholars also receive additional support from Wang-Cai Biochemistry Lab Donation Fund. SciEcon wholeheartedly supports DKU’s noble mission of advancing interdisciplinary research and fostering integrated talents. Our support is solely focused on promoting academic excellence and knowledge exchange. SciEcon does not seek any financial gains, property rights, or branding privileges from DKU. Moreover, individuals involved in this philanthropy event perform their roles independently at DKU and SciEcon.

**Keywords(hashtags)**
================

\#Crypto Exchanges \#Centralized Exchanges \#Decentralized Exchanges \#Transaction \#Transaction fee \#Trading volume \#ETH Token \#Incident

**Highlights:**
================
1. Research: The article explores the trading of ETH tokens on centralized exchanges (CEXs) and decentralized exchanges (DEXs) in the cryptocurrency market, compares the various trading indicators, analyzes the correlation and causality, and helps to explore the factors affecting the trading status of cryptocurrency exchanges and is useful for studying the development trend of the cryptocurrency market.
2. Innovation: The article takes the collapse of FTX as an event, selects two months before and after the event as time points, and adopts a quantitative research method to study the Granger causality among transaction data to explore the impact of the event on cryptocurrency exchanges, and to provide a reference for the future development of the cryptocurrency market.
3. Leadership: In the article, we analyze the impact of the event and the market reaction, analyze the relevant, easy anger which affects the trading status of cryptocurrency exchanges, and further explore the specific impact of the event on the market and user choice. The article provides guidance and insights for leaders and decision-makers to better respond to market dynamics and risks.

**Supplementary Code:**
================
The open code resources are available on GitHub: https://github.com/SciEcon/SRS2023_cex_dex

*Please refer to the GitHub Page for detailed code about the data collection and processing.*


![](https://miro.medium.com/v2/resize:fit:1400/format:webp/1*_Ofi18M7tjOvTxExkClVxA.png)<br />Figure  1: Article Flow Chart (created by Whimsical).

**Introduction**
================

In previous studies on cryptocurrency exchanges, the focus was on comparing two common cryptocurrency exchanges, [centralized exchange (CEX)](https://101blockchains.com/centralized-crypto-exchange/) [1] and [decentralized exchange (DEX)](https://chain.link/education-hub/what-is-decentralized-exchange-dex) [2], to explore users’ tendency to choose and trust these two exchanges. Through the comparison of four aspects: transaction process and mechanism, advantages and disadvantages, literature review, and actual market characteristics, we noticed a purely theoretical qualitative study is difficult to confirm the factors which affect the number of users and transaction volume of cryptocurrency exchanges, and further confirmation is needed from a quantitative study supported by actual transaction data.

The project takes the [ETH token](https://etherscan.io/) [3] as an example by selecting two months before and after the [FTX collapse](https://www.investopedia.com/what-went-wrong-with-ftx-6828447) [4] (November 11th, 2022) as the time nodes to analyze the transaction indicators such as transaction volume (in USD), transaction fees, and transactions in CEX and DEX, investigate the correlation between the indicators, explore users’ preference for CEX and DEX, and provide the development direction for future cryptocurrency exchanges. First, the research analyzed the ETH token flow of CEX and DEX, considering the migration in both inflow and outflow directions, and presented the changes of each transaction indicator over time by drawing a graph. Then, we performed the correlation test and [Granger causality](http://www.scholarpedia.org/article/Granger_causality) [5] test ([Engle and C. W. J. Granger 1987](https://www.ntuzov.com/Nik_Site/Niks_files/Research/papers/stat_arb/EG_1987.pdf)) for the data analysis of the trading indicators therein. Also, the analysis of liquid trading between CEX and DEX focused on the changes in trading indicators before and after the FTX collapse incident. Finally, we summarize the above findings, provide a comprehensive overview of CEX and DEX transactions, and analyze the future direction of cryptocurrency exchanges, thus proposing a possible collaborative system between centralized and decentralized finance. ([Qin et al. 2021](https://arxiv.org/abs/2106.08157)). The study helps users understand the cryptocurrency market better and supports informed decision-making by examining the trends between the CEX and DEX platforms and their distribution.

![](https://miro.medium.com/v2/resize:fit:1400/format:webp/1*cgCu3Ku3zA2vbCIah4QZ_Q.png)<br />Figure  2: Decision tree (created by Whimsical).


**Data Exploration**
================
Part 1. Data Collection
============

The study collected data at [Flipside Crypto](https://flipsidecrypto.xyz/) [6] and collected data for 61 days from October 11th,2022, to December 11th,2022, obtained on June 28th,2023.

In the query phase, obtained the inflows and outflows of ETH tokens on CEX and DEX separately, including the transaction volumes, transactions, and transaction fees. We also obtained the metrics of the flow of ETH tokens between CEX and DEX, including the number of users, transaction volume, transactions, and transaction fees. Major transaction CEXs include [Coinbase](https://www.coinbase.com/), [SwissBorg](https://swissborg.com/), [Binance](https://www.binance.com/), [Kraken](https://www.kraken.com/), [Hotbit](https://www.hotbit.io/), [Ethfinex](https://www.crunchbase.com/organization/ethfinex), [IDEX](https://idex.io/), [Crypto.com](https://crypto.com/), and [Kucoin](https://www.kucoin.com/). Major transaction DEXs include [Uniswap](https://uniswap.org/), [Balancer](https://balancer.fi/), [1inch](https://app.1inch.io/), [Curve](https://curve.fi/), [Sushiswap](https://www.sushi.com/), [0x](https://0x.org/), [ParaSwap](https://www.paraswap.io/), [CoW Swap](https://swap.cow.fi/), [ShibaSwap](https://shibaswap.com/), and [MetaMask](https://metamask.io/).

In the process phase, we obtained the overall transaction metrics of CEX and DEX, including total transaction volume, total transactions, and total transaction fees, by integrating the original data collected in the query phase.


![](https://miro.medium.com/v2/resize:fit:1400/format:webp/1*gznMQZKyDCMdJ5XPe8xQ6A.png)<br />Figure  3: Data dictionary (created by GitHub).

![](https://miro.medium.com/v2/resize:fit:1400/format:webp/1*klLvWx7I_W_wbuz7EE8-9Q.png)<br />Figure  4: Top 10 exchanges by transaction volume (data from Flipside Crypto, created by Miro).

Part 2. Data Visualization
============
Based on the collected and organized data, we wrote code on Google Colab for data visualization. And we plotted the total transaction volume line chart, total transaction cost line chart, total transaction volume-transaction cost line chart, and total transaction cost-transaction line chart for CEX and DEX. We also plotted comparative line graphs of asset flows between CEX and DEX, including the number of users, transactions, transaction fees, and transaction volumes.

![](https://miro.medium.com/v2/resize:fit:1400/format:webp/1*dITAO-xlu1T-FzsctudnWw.png)<br />Figure  5: CEX Visualization (created by Google Colab).

![](https://miro.medium.com/v2/resize:fit:1400/format:webp/1*Z69fS0bcaG6YmQCiHLaB8Q.png)<br />Figure  6: DEX Visualization (created by Google Colab).

![](https://miro.medium.com/v2/resize:fit:1400/format:webp/1*XJmjJHT4ZKJtx7cMpoyjDA.png)<br />Figure  7: CEX and DEX Flow Visualization (created by Google Colab).


Part 3. Data Analysis
============
The research first examined the correlation between transaction volume and transaction fees and between transaction fees and transactions for ETH tokens on CEX and DEX. The correlation coefficient between transaction volumes and transaction fees on CEX is 0.32, which is relatively weak, while the correlation coefficient between transaction volumes and transaction fees on DEX is 0.65, which is relatively strong.

Due to the large gap between the correlation test data of transaction volumes and transaction fees on CEX and DEX, we calculated another indicator, the Granger causality test. The test is used to determine whether a causal relationship exists between two-time series. If the past values of one time series (X) can predict the current values of another time series (Y), and the past values of Y do not have predictive power for the current values of X, then we can assume X has a causal effect on Y. ([Engle and C. W. J. Granger 1987](https://www.ntuzov.com/Nik_Site/Niks_files/Research/papers/stat_arb/EG_1987.pdf)). The research first collected data from two-time series, transaction fees, and transaction volumes. Then, we concluded by constructing an [Autoregressive model (ARM)](https://en.wikipedia.org/wiki/Autoregressive%E2%80%93moving-average_model) [7] to compare the model prediction errors. We reject the hypothesis of Granger causality between the transaction volumes and transaction fees in CEX and DEX. Ante et al. also conducted Granger causality tests on transaction fees and transaction volumes when studying blockchain activity in the Ethereum blockchain network. ([Ante and Saggu 2023](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=4400040)). The results show a lack of consistent Granger causality between Ethereum transaction fees and transaction volumes. Multiple factors such as market sentiment, trading opportunities, and expansion of the DeFi ecosystem influence user behavior, not just transaction fees. Therefore, we consider the impact of the FTX collapse on the cryptocurrency trading market.

By looking at the graphs of the number of users, transactions, transaction fees, and the transaction volumes flowing between CEX and DEX obtained from the data visualization, we have the following four discoveries.:

**The number of users**

Before November 11th, 2022, the number of users from DEX to CEX was more than the number of users from CEX to DEX. But in the 20 days after November 11th, 2022, there were three data changes, and the number of users from CEX to DEX became more. We speculated the situation may be because the FTX collapse event facilitated the loss of CEX users.

**Transactions**

Before November 11th, 2022, DEX to CEX transactions was almost equal to CEX to DEX transactions. However, in the 30 days after November 11th, 2022, there were significantly more asset transfers from CEX to DEX than from DEX to CEX. Presumably, the situation may be due to the FTX collapse incident prompting users to transfer assets from CEX to DEX.

**Transaction Fees**

Before November 11th, 2022, DEX-to-CEX transactions were nearly equivalent to CEX-to-DEX transactions. However, in the 20 days after November 11th, 2022, the transaction fees from CEX to DEX were significantly higher than transaction fees from DEX to CEX. The situation may be because the FTX collapse event prompted user trading activity from CEX to DEX, and the increased demand in the market caused some network congestion, resulting in higher transaction fees. The stronger correlation between transaction costs and trading is also verified here.

**Transaction volumes**

Before November 11th, 2022, DEX to CEX transaction volumes were consistently higher than CEX to DEX volumes. However, in the 20 days after November 11th, 2022, the volume of DEX to CEX decreased significantly and even equaled the volume of CEX to DEX on November 19th, 2022. The reason for the situation may be due to the loss of assets of users caused by the FTX collapse, the cooling of the market, and the lower level of economic activity. We also confirm what was previously found during the actual market research, nine of the top 10 cryptocurrency exchanges concerning trading volume are CEX, and only 1 is DEX. Despite the impact of the FTX collapse, CEX still dominates the cryptocurrency exchanges.


**Conclusion & Discussion**
================
In the article, by analyzing the trading metrics of specific tokens in CEX and DEX, we can have the following conclusions:

1. CEX is more popular among the actual cryptocurrency exchanges, with more users and larger transaction volumes.

2. There is a strong correlation between transaction fees and trading. The increase in transactions reflects the dynamism of the market, leading to higher transaction fees, which may be moderated by fewer transactions when transaction fees rise to a certain level.

3. In addition to transaction fees, transaction volume is impressed by multiple factors. Current economic conditions, market heat, or unexpected events may have some impact on the trading volume of an exchange, and the analysis of trading volume needs to be considered holistically.

![](https://miro.medium.com/v2/resize:fit:1400/format:webp/1*PMhs2i523IKpKyraF3WRYA.png)<br />Figure  8: Findings (created by Whimsical).

The current market status and user preferences of CEX and DEX are inseparable from the economic system. In a comparative study on [centralized finance (CeFi)](https://www.coinbase.com/learn/crypto-basics/what-is-cefi) [8] and [decentralized finance (DeFi)](https://ethereum.org/en/defi/) [9], Qin et al. analyze their technological differences, economic differences, and legal characteristics and suggest some possible synergies. ([Qin et al. 2021](https://arxiv.org/abs/2106.08157)). Their study argues CeFi and DeFi intertwine and improve each other as two different financial systems. For example, financial institutions bridge CeFi and DeFi through [oracles](https://chain.link/education-hub/what-is-an-automated-market-maker-amm) [10] to improve efficiency; the [automatic market maker (AMM)](https://chain.link/education-hub/what-is-an-automated-market-maker-amm) [11] trading mechanism introduced by DeFi replaces CeFi’s order book model, inspiring CeFi to start providing market-making services using a similar model; and the lessons provided by the DeFi collapse on CeFi as well as stress testing. There is mutual absorption between CeFi and DeFi innovation and learning from each other, and these two financial models exhibit different characteristics and challenges under different market conditions. Suppose the industry can propose a collaborative financial system based on these two financial models to provide high-quality financial products and services to users.

The study reveals the differences between centralized and decentralized cryptocurrency exchanges, emphasizing the importance of quantitative research to complement qualitative analysis. Examining transaction data, correlations, and trends provides a more comprehensive understanding of user preferences and the dynamics of the CEX and DEX platforms. The research provides insights into asset flows, user behavior, and market reactions, particularly to the FTX collapse. However, there are some limitations to consider. The focus of the study is on ETH token trading, and the findings may not be generalizable to other cryptocurrencies. The period chosen and the specific event (FTX collapse) may affect the observed results, and caution should be exercised in drawing broad conclusions. In addition, the analysis relies on data available from Flipside Crypto and may not capture the entire cryptocurrency market.

In future research, we would like to extend the analysis to a broader range of cryptocurrencies and examine other factors which influence user preferences and trust in cryptocurrency exchanges. Exploring the role of regulatory frameworks, security measures, and user experience could provide further insights into the development of the CEX and DEX platforms. Furthermore, given the evolving cryptocurrency market, continuous monitoring and analysis of market trends and user behavior are critical to understanding the emerging patterns and dynamics of the industry.

**Relevant Materials**
================

\[1\] centralized exchange (CEX)

A centralized cryptocurrency exchange (CEX) is an online platform that facilitates the buying, selling, and trading of cryptocurrencies. Operating under a central entity, CEXs provide a user-friendly interface and offer features like high liquidity, various trading options, and security measures to protect user funds.

[Website — what is CEX](https://101blockchains.com/centralized-crypto-exchange/)

\[2\] decentralized exchange (DEX)

A decentralized exchange (DEX) is a peer-to-peer platform that enables direct cryptocurrency trading without intermediaries. It operates on a decentralized network, allowing users to maintain control of their funds and trade directly with others, promoting transparency, privacy, and eliminating the need for trust in a central authority.

[Website — what is DEX](https://chain.link/education-hub/what-is-decentralized-exchange-dex)

\[3\] ETH token

ETH token, also known as Ethereum, is a decentralized digital currency. ETH is a widely recognized and widely used cryptocurrency, offering programmable money and fostering innovation in the blockchain space.

[Ethereum — ETH](https://ethereum.org/en/eth/)

\[4\] FTX collapse

On November 11, 2022, FTX Trading, a well-known cryptocurrency trading platform, announced FTX and other FTX Group subsidiaries had initiated voluntary bankruptcy proceedings under relevant U.S. laws.

[News — FTX collapse](https://www.investopedia.com/what-went-wrong-with-ftx-6828447)

\[5\] Granger causality

Granger causality is a statistical concept of causality based on prediction. According to Granger causality, if a signal Y1 “Granger-causes” a signal Y2, then past values of Y1 should help to predict Y2 above and beyond the information contained in past values of Y2 alone.

[Wikipedia — Granger causality](https://en.wikipedia.org/wiki/Granger_causality)

\[6\] Flipside Crypto

Flipside Crypto is a leading blockchain data analytics firm. Flipside Crypto provides actionable insights and analytics for investors, traders, and blockchain projects, leveraging on-chain and off-chain data to offer a comprehensive analysis of token economics, user behavior, and market trends.

[Website — Flipside Crypto](https://flipsidecrypto.xyz/)

\[7\] Autoregressive model (ARM)

The autoregressive model (ARM) is a time series analysis method used to predict the relationship between past observations and current observations of a variable.

[Wikipedia — Autoregressive model (ARM)](https://en.wikipedia.org/wiki/Autoregressive%E2%80%93moving-average_model)


\[8\] centralized finance ( CeFi )

Centralized Finance (CeFi) refers to a centralized traditional financial system and relies on intermediaries such as centralized exchanges and banks. CeFi operates under the trust of third-party entities and provides various financial services and trading facilities.

[Coinbase — CeFi](https://www.coinbase.com/learn/crypto-basics/what-is-cefi)

\[9\] decentralized finance ( DeFi )

Decentralized Finance (DeFi) refers to a financial ecosystem built on blockchain technology. The DeFi aims to eliminate intermediaries and provide open, permissionless financial services to anyone with an internet connection. DeFi encompasses various decentralized applications (DApps) offering services like lending, borrowing, trading, and yield farming.

[Ethereum — Defi](https://ethereum.org/en/defi/)

\[10\] Oracle

Blockchain oracles connect blockchains to external systems, enabling smart contracts to access real-world data and interact with traditional systems. Oracles facilitate the creation of hybrid smart contracts which combine on-chain code with off-chain infrastructure, empowering decentralized applications to respond to real-world events and interoperate with existing systems.

[Chainlink — Oracles](https://chain.link/education/blockchain-oracles)

\[11\] Automated Market Maker (AMM)

An Automated Market Maker (AMM) is a decentralized protocol. The AMM enables the automated trading of cryptocurrencies without relying on traditional order books. The AMM uses smart contracts to provide liquidity and facilitate trades based on predetermined mathematical algorithms and pools of funds.

[Chainlink — AMM](https://chain.link/education-hub/what-is-an-automated-market-maker-amm)



**About the Author**
================
**Xintong Wu**
![](https://miro.medium.com/v2/resize:fit:1400/format:webp/1*RXkBlhUQe751O0O204NlBA.jpeg)<br />Figure 5: Xintong Wu.

*Xintong Wu* is a student in the Class of 2025 at Duke Kunshan University, majoring in Computation and Design. Her interests are digital design, digital market research, and metaverse. She hopes to delve into the dynamic interactions between technology and society in the future Web 3.0 era and explore the infinite possibilities that technology can bring. Through the research with Prof. Luyao Zhang, she hopes to create new digital virtual worlds of diversity, interdisciplinarity, and infinite possibilities.

**Acknowledgments**
================
My sincere appreciation to SciEcon Insights and its directors:

**Interim Executive Editors**: Wanlin Deng, Yutong Quan

**Associate Editor**: Xinyu Tian

**Chief Editor**: Prof. Luyao Zhang

**Design**: Yixuan Li
