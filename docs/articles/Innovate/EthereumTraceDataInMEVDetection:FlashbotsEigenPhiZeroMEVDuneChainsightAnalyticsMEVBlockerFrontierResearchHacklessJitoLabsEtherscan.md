**Ethereum Trace Data in MEV Detection: Flashbots, EigenPhi, ZeroMEV, Dune, ChainsightAnalytics, MEV Blocker, Frontier Research, Hackless, Jito Labs, Etherscan**
======================
> **Disclaimer:** This article is a final deliverable from Prof. Luyao Zhang’s project entitled “From ‘Code is Law’ to ‘Code and Law’: A Comparative Study on Blockchain Governance,” supported by the 2023 Summer Research Scholarship (SRS) program at Duke Kunshan University. Our Summer 2023 scholars also receive additional support from Wang-Cai Biochemistry Lab Donation Fund. SciEcon wholeheartedly supports DKU’s noble mission of advancing interdisciplinary research and fostering integrated talents. Our support is solely focused on promoting academic excellence and knowledge exchange. SciEcon does not seek any financial gains, property rights, or branding privileges from DKU. Moreover, individuals involved in this philanthropy event perform their roles independently at DKU and SciEcon.

**Keywords:**

#MEV #Cryptocurrency #Machine Learning #DeFi #Python

**Highlights:**

* Research: Conduct research on exporting transaction/trace data
* Innovation: Identify simple Python code to export transaction data
* Leadership: Provide new dataset for MEV analysis, and find limitations for future study
# Supplementary Code
The supplementary code in the article is released as open access on GitHub: https://github.com/SciEcon/SRS2023_MEV_Jay
# Introduction
Miner Extractable Value (MEV) poses a pressing concern in the cryptocurrency world, offering profit opportunities to miners through transaction reordering, front-running, and censorship on the blockchain [(“Miner Extractable Value (MEV),” n.d.)](https://ethereum.org/en/developers/docs/mev/). According to [​​Piet, Fairoze, and Weaver (2022)](https://arxiv.org/abs/2203.15930), [Flashbots](https://explore.flashbots.net/?ref=blog.pantherprotocol.io), and [Qin, Zhou, and Gervais (2022)](https://ieeexplore.ieee.org/abstract/document/9833734?casa_token=lK51OU_i5GUAAAAA%3A4FJ3dfKPGNq12PoBetN_yVk3D49BmZNLF2tIeeQkiZe_hYtqlLv87fSYWuN5MqskEcmPuIDr), traditional methods of identifying MEV-affected transactions through manual data collection and heuristics may become inadequate as transaction complexity grows. Thanks to [Etherscan](https://etherscan.io/), the website has provided MEV data for each transaction that everyone can access easily. In industry, [EigenPhi](https://eigenphi.io/) helps companies and projects in the blockchain space optimize their operations, mitigate the risks associated with MEV, and identify novel strategies to maximize their economic gains through their innovative approach. By leveraging advanced algorithms, data analytics, and deep domain expertise, EigenPhi empowers its clients to navigate the complex landscape of MEV and make informed decisions to stay competitive in the rapidly evolving blockchain industry. Moreover, [Flashbots](https://www.flashbots.net/), [Frontier Research](https://www.frontiersin.org/), [ZeroMev](https://zeromev.org/), [Dune](https://dune.com/home), and [Bitquery](https://bitquery.io/) are aiming to foster a more transparent, robust, and equitable DeFi ecosystem, where users can participate without concerns of MEV exploitation. Under the framework of Dune, [ChainsightAnalytics](https://dune.com/ChainsightAnalytics) works as one of the most important tools to detect new MEV attacks and allow analysts to focus on previously overlooked fields. Furthermore, besides these websites which mainly work for the chain Ethereum, [Jito Labs](https://www.jito.wtf/) has made a great contribution to the chain Solana and [introduced the First Solana MEV Dashboard](https://www.jito.wtf/blog/introducing-the-first-solana-mev-dashboard/) there. Additionally, [Hackless](https://hackless.io/) concentrates on protecting users in EVM with their MetaMask Wallet from MEV attacks. By collaborating with industry partners, contributing to academic discussions, and developing innovative technologies, the three platforms continue to be a driving force in shaping the future of MEV research and solutions in the blockchain space.
| Website | GitHub |Database and Open API |Event | Research | The focus area of MEV |
| ------------- | ------------- |------|------|--------|------|
| EigenPhi(https://eigenphi.io) | https://github.com/eigenphi | Public as open source(https://eigenphi-1.gitbook.io/classroom/communities-and-channels/our-mev-daily-report/download-and-share-daily-report-data) | EigenPhi workshop(https://eigenphi.substack.com/p/defi-daily-digest-2022-09-05-tools#§mev) | EigenPhi in Substack(https://eigenphi.substack.com) | It provides the best analytical tools detailing MEV and liquidity on-chain data, as well as bespoke research to allow analysts, institutions,  traders, protocols、 and any DeFi stakeholders to accurately see the on-chain behaviors, structures, and networks leading to arbitrage, sandwich attacks, malicious tokens and liquidations impacting their interests.(https://eigenphi-1.gitbook.io/arbitrage-scan-user-guide/) |
| ZeroMEV(https://zeromev.org) | https://github.com/zeromev/zeromev-geth|Public as open source(https://info.zeromev.org/api)| N/A| Zeromev-Geth: Unilateral Fair Ordering(https://info.zeromev.org/zmgeth-proposal.html)| It protects and empowers the Ethereum community against frontrunning and censorship. It also provides Ethereum researchers and users with detailed info on MEV and transaction reordering on the Ethereum blockchain.(https://info.zeromev.org/technical.html#extractor-service)|
| Frontier Research(https://frontier.tech/)| N/A|N/A| Official twitter(https://twitter.com/FrontierDotTech)|Exploration of MEV Latencies(https://frontier.tech/exploration-of-mev-latencies)|An independent research and advisory group formed to bridge the gap between fundamental research and commercial products. We build upon our expertise in MEV and blockchains to pull the future of crypto into reality.|
| Flashbots(https://www.flashbots.net)| https://github.com/flashbots|  Public as open source(https://flashbots-data.s3.us-east-2.amazonaws.com/index.html), API(https://docs.flashbots.net/flashbots-data/blockapi) | Workshops(https://github.com/flashbots/mev-research/blob/main/workshops.md)|Flashbots in Medium(https://medium.com/flashbots)| Illuminate: bringing transparency to MEV activity. Democratize: democratizing access to MEV revenue. Distribute: enabling sustainable distribution of MEV revenue.(https://www.flashbots.net)|
|Bitquery(https://bitquery.io)|https://github.com/bitquery|Public with subscription plan(https://bitquery.io/pricing)Trace Data(https://docs.bitquery.io/docs/examples/calls/smartcontract_filterby/#smart-contract-calls-by-arguments)|Bitquery workshop(https://www.eventbrite.com/e/bitquery-workshop-1-w-metricsdao-tickets-625155606247)|Bitquery in Medium(https://medium.com/bitquery)| An API-first product company dedicated to power and solve blockchain data problems, including MEV, using the ground truth of on-chain data(https://bitquery.io/about)|
|Dune(https://dune.com/home)|https://github.com/DuneAnalytics|Public with subscription plan(https://dune.com/cowprotocol/mev-blocker)|Dune Youtube workshop(https://www.youtube.com/channel/UCPrm9d2hLd_YxSExH7oRyAg)|Dune Analytics: An Overview of Blockchain Top Data Plug(https://medium.com/coinmonks/dune-analytics-an-overview-of-blockchain-top-data-plug-dd51001a5408)|A web-based platform that allows us to query public blockchain data, analyze MEV data, and aggregate it into beautiful dashboards.(https://dune.com/cowprotocol/mev-blocker)|
|MEV Boost Dashboard(https://mevboost.pics)| https://github.com/Nerolation/mevboost.pics| Public as open source(https://mevboost.pics/data.html)| N/A| N/A| Track MEV-Boost relays and blockbuilders. Users can monitor network participation rates and Flashbot dominance with it, while also top builders and relays. It also provides an API that aggregates data across tracked relays. (https://www.alchemy.com/dapps/mev-boost-analytics)|
|Jito Labs(https://www.jito.wtf)|https://github.com/jito-labs |Public with subscription plan(https://web.miniextensions.com/WV3gZjFwqNqITsMufIEp)| Jito Labs workshop(https://solana.com/breakpoint)| Jito Labs in Medium(https://jito-labs.medium.com) Now moved to Jito Labs Blog(https://www.jito.wtf/blog/)| Make Solana more efficient, minimize the negative impact of MEV on users, maximize MEV returned to users and stakers(https://jito-foundation.gitbook.io/mev/solana-mev/jitos-mev-priorities)|
| Hackless(https://hackless.io)| N/A |N/A |N/A |Hackless Blog(https://hackless.io/blog) Hackless in Medium(https://medium.com/@hackless)| Provide a comprehensive security layer for DeFi protocols, with solutions for mitigating risks, decreasing losses, and preventing potential attacks. It offers services such as SafeMigrate for migrating funds from paused DeFi protocols, Watchdog for ongoing monitoring and prevention of fraudulent transactions, and Conductor for private mining.(https://www.alchemy.com/dapps/hackless)|
Table 1, Top websites in dealing with MEV issues

Table 1 presents some top websites for dealing with MEV issues. The table includes these websites’ services, research, events, and focus areas of MEV with links.

This exploratory research article aims to explore the potential of using machine learning techniques and new datasets to enhance MEV detection. By analyzing vast amounts of transaction data and learning from historical MEV occurrences, machine learning algorithms can adapt and provide more efficient, accurate, and automated solutions for detecting MEV, thereby ensuring a more robust and reliable detection mechanism.
|Variable name|Explanation|
|----|----|
|Block|The block number in which the transaction was included|
|Timestamp|The time the transaction happens|
|Transaction Hash|The hash of the transaction that generated this trace|
|From|The Ethereum address of the sender (originating address) of the transaction.|
|To|The Ethereum address of the recipient (destination address) of the transaction. It can be None if the transaction is creating a new contract|
|Nounce|Number of the transactions made by the sender prior to this one|
|Value|The value transferred in Wei|
|Gas|Gas provided by the sender|
|Gas Price|The gas price provided by the sender in Wei|
|Receipt cumulative|The total amount of gas used when this transaction was executed in the block|
Table 2. Transaction DataFrame Variables Explanation.

As shown in Table 2, these headers are included in the transaction data, which refers to the information associated with individual transactions on the Ethereum blockchain. The data reflect the details and characteristics of individual transactions, such as who sent/received Ether, the value transferred, and the smart contract interactions performed.
# Traces
In this article, based on previous research, we want to introduce trace data into machine learning in MEV detection. Trace data also attaches much importance to the blocks apart from the transaction data. Each transaction execution generates a trace, which includes various operations and sub-operations performed during the transaction execution, and thus trace data provides a more detailed and low-level view of the execution of transactions and smart contracts on the Ethereum blockchain. This article will focus on analyzing Cryptocurrency Ethereum Traces data. The dataset contains over 7.2 billion rows since 2016.
|Variable name|Explanation|
|---|----|
|transaction_hash|The hash of the transaction that generated this trace|
|transaction_index|The index of the transaction within the block in which it was included|
|from_address |The Ethereum address of the sender (originating address) of the transaction.
to_address,The Ethereum address of the recipient (destination address) of the transaction. It can be None if the transaction is creating a new contract|
|value|The value of Ether (ETH) transferred in the transaction|
|input|The input data for the transaction, typically containing the function signature and parameters for a smart contract function call|
|output|The output data produced by the transaction is often empty unless it's a contract creation or function call that returns data|
|trace_type|Indicates the type of trace. Possible values include 'call', 'create', 'suicide' and others|
|call_type|Indicates the type of call made by the trace. Possible values include 'call', 'delegate_call', 'static_call', and others|
|reward_type|Indicates if the trace is related to mining rewards|
|gas|The gas limit specified in the transaction|
|gas_used|The amount of gas used by the trace|
|subtraces|The number of subtraces generated by the trace|
|trace_address|A list of integers representing the path through the call trace tree|
|block_timestamp|The timestamp when the block containing the transaction was mined|
|error|Contains error information if the transaction execution resulted in an error|
|status|Indicates the status of the transaction. Possible values are 1 for success and 0 for failure|
|block_number|The block number in which the transaction was included|
|block_hash|The hash of the block in which the transaction was included|
Table 3. Trace DataFrame Variables Explanation.

Table 3 explains the headers of contents included in trace data. Usually, to apply the dataset for further study, we first need to filter data with ‘Status’ equal to ‘1’, ensuring that the transaction is successful.

Trace data allows developers and researchers to analyze how smart contracts are executed and interact with each other on the Ethereum network. It includes information about function calls, contract creations, and contract self-destructs, among other operations. [*What is Ethereum Trace?*](https://community.bitquery.io/t/bitquery-trace-api/1556?u=divya#what-is-ethereum-trace-1) has pointed out that an Ethereum Virtual Machine (EVM) trace is a comprehensive record of the steps taken by the EVM to execute a transaction, providing details like gas consumption, step results, and encountered errors. EVM traces serve multiple purposes, making them a valuable tool for developers and researchers. They are instrumental in debugging smart contracts, analyzing performance, and identifying potential security vulnerabilities. To understand the workings of smart contracts, EVM traces can be used to follow the flow of funds on the Ethereum blockchain and identify potential security issues, just as shown in Figure 1.
![](https://miro.medium.com/v2/resize:fit:1400/format:webp/1*UBObleVewlJc62tKcQWLAg.png)
Figure 1. [Sample Token Flow.](https://eigenphi.io/)

For visualization, a CallTrace Tree for a specific transaction is also constructed. The call tree starts with the root node representing the main function of the smart contract. It has child nodes, such as “burn” and “positions,” which represent functions called within the contract. Some nodes have further child nodes, illustrating multiple calls to different functions within the same or different smart contracts.
![](https://miro.medium.com/v2/resize:fit:788/format:webp/1*epUeHTJe2s8YidGz3pTrAQ.png)
Figure 2. [The Composition of a CallTrace Tree.](https://community.bitquery.io/t/bitquery-trace-api/1556?u=divya#what-is-ethereum-trace-1)

![](https://miro.medium.com/v2/resize:fit:1400/format:webp/1*d4EhYuG-0KHy05AGTi9Xfw.png)
Figure 3. [An Example of CallTrace Tree.](https://eigenphi.io/)

Figure 2 has illustrated a normal composition of a CallTrace Tree and Figure 3 shows an example. We can understand what each transfer does under the framework of CallTrace Tree.

Analyzing EVM traces can reveal unintended function calls within smart contracts. In some cases, miners can trigger certain functions unexpectedly, potentially leading to undesired outcomes or financial losses for users. Detecting these unintended function calls requires analyzing the traces of transactions involving the affected smart contracts. By merging the trace data with MEV Blocker data retrieved from Dune, it may enable us to label the problematic trace routes as well as the MEV-affected transactions, warning users.
# Literature Review
In previous research, [Heimbach et al. (n.d.)](https://arxiv.org/pdf/2305.19037.pdf) have used trace data to compare the target transaction addresses with a list of sanctioned addresses from [OFAC](https://www.treasury.gov/ofac/downloads/sanctions/1.0/sdn_advanced.xml). This process helps them gain insights into non-compliant transactions that may violate OFAC regulations and other sanctions. Meanwhile, [Heimbach et al. (n.d.)](https://arxiv.org/pdf/2302.06708.pdf) aim to gain insights into the parallelizability of the Ethereum mainnet workload by studying the trace data. Analyzing trace data helps them understand how efficiently the Ethereum network can process multiple transactions in parallel and how this capability has evolved over time. By examining historical and recent data, they seek to identify patterns and trends that can provide valuable information about the scalability and performance of the Ethereum blockchain. According to another research [(Wahrstätter et al. n.d.)](https://arxiv.org/abs/2305.16468), by employing trace data, the authors map Ethereum addresses to identified entities to provide a more comprehensive picture of the Ethereum ecosystem, thus enabling deeper analysis of participant roles and relationships.
# Retrieve Data
[Ethereum ETL](https://github.com/blockchain-etl/ethereum-etl) has provided us with an open public dataset in Google BigQuery. The dataset updates periodically and allows us to access the latest trace data in the blockchain.
![](https://miro.medium.com/v2/resize:fit:1032/format:webp/1*9luj7clEzxmXv2bioYt6Mg.png)
Figure 4. Crypto_Ethereum public dataset.

Figure 4 has shown part of the public datasets that ethereum_etl provides.

To query the SQL workspace in Google BigQuery, using Kaggle is a good way to meet the requirements.
![](https://miro.medium.com/v2/resize:fit:1400/format:webp/1*rv3JlEKV6rx4STqC0RczBw.png)
Figure 5. Google SQL BigQuery code.

As shown in Figure 5, the code can export data in public datasets into our own workspace. Note that since the original dataset is too big, we have to transfer data several times by adjusting the time range.
![](https://miro.medium.com/v2/resize:fit:1400/format:webp/1*5Cyy_4qN8K627kVCSV084g.png)
Figure 6. Sample Kaggle output.

The code in Figure 6 will export our data in the SQL table into Google Cloud Storage (GCS) in the format of CSV files, making the data available for download.
![](https://miro.medium.com/v2/resize:fit:1400/format:webp/1*WKVlMN6-vvfXK_RATOMsmQ.png)
Figure 6. Exported Datasets in Private GCS.

Figure 6 is a preview of exported files in our own Google Cloud Storage. These files can be downloaded directly.
![](https://miro.medium.com/v2/resize:fit:1400/format:webp/1*qp5abITGD_Mh3sl26SDqoA.png)
Figure 7. Sample trace data.

Figure 7 shows the sample data we produced in CSV format.
![](https://miro.medium.com/v2/resize:fit:1400/format:webp/1*UpL3l7y1t1vezdfP-SRu0A.png)
Figure 8. The number of successful traces each month over time.

As shown in Figure 8, the count of traces is generally increasing, and the rapid drop at the end is due to only half of the transactions in July 2023 being counted.

https://github.com/SciEcon/SRS2023_MEV_Jay/blob/main/code/MEVblocker_data_query.ipynb

The upper link provides a sample code for querying MEV blocker data from [Dune](https://dune.com/cowprotocol/mev-blocker). Limited by the website and the free API plan we use, we only export 100 rows of data. By using [Dune Client](https://github.com/cowprotocol/dune-client) developed by Dune with a subscription plan, we are allowed to access more data.
![](https://miro.medium.com/v2/resize:fit:1400/format:webp/1*xNfj_0Ru-v6d7mL2ibGFMQ.png)
Figure 9. MEV blocker proportion over time.

Figure 9 is a stack area diagram drawn from the data retrieved from the code above. The y-axis of the figure represents the proportion of transactions protected by the MEV blocker among all the transactions, and the proportion is showing an increasing trend from April 24th, 2023 to August 2nd, 2023.
# Conclusion & Future Direction
Using Cryptocurrency Ethereum Traces data to detect MEV has provided a new method for relative research, enabling us to label MEV-affected transactions from a new angle. However, we still fail to label the potential MEV-affected transactions before the transaction completes, being recorded on the blockchain. Using data like Node Tracker from Etherscan (5000-download limited each time) can possibly detect MEV earlier and stop the transaction if necessary. Sadly, there is no open data currently, and we are forced to collect incomplete data from our peers in Geth, OpenEthereum, and so on. It is hard to collect the complete data for research.
![](https://miro.medium.com/v2/resize:fit:1400/format:webp/1*3Ol2W-HYgmNOiSIlSiKrKw.png)
Figure 9. Number of Occurrences for Each Country.
![](https://miro.medium.com/v2/resize:fit:1400/format:webp/1*SDlKCzGYO-y5X8Q_WzkUug.png)
Figure 10. Circle Plot for Top 5 Countries and Their Occurrences.

Due to the limitations and policies of [Etherscan](https://etherscan.io/), users can only export 5,000 sets of Node Tracker data each time, making users unable to export the whole daily Node Tracker data, which is normally over 7,000. In this case, according to the incomplete Node Tracker data, precisely 13,983 rows, exported from July 22nd, 2023 to July 29th, 2023, we can obtain Figure 9 and Figure 10. As illustrated in Figure 9, it tells us the number of occurrences for the users’ IP addresses. Users from many different countries are trading on the blockchain but are mainly concentrated in the US, Germany, and the UK. Based on this information, in Figure 10, we primarily want to compare the top 5 countries. The bigger the blue circle is, the more occurrences of a country’s IP address have been recorded. The US takes a commanding lead, showing its great passion for the cryptocurrency market.

In conclusion, this exploratory research article extensively explores the potential of leveraging machine learning techniques and Ethereum Trace data to significantly enhance the detection of MEV in cryptocurrency transactions. The incorporation of trace data, providing intricate insights into transaction executions and smart contract interactions, has facilitated a more comprehensive analysis of MEV activities. One limitation encountered in this research is the incapacity to label potential MEV-affected transactions before their recording on the blockchain. To potentially detect MEV earlier and prevent undesired outcomes, the utilization of data such as Node Tracker from Etherscan appears promising. However, the scarcity of accessible open data sources for this specific purpose has posed challenges in acquiring sufficient and complete data. Despite these obstacles, this exploratory research article contributes to advancing MEV detection methodologies and deepening our understanding of the impact of MEV on the cryptocurrency ecosystem.

To continue refining MEV detection and mitigating its effects in the constantly evolving realm of cryptocurrencies, further research and collaborative efforts to obtain comprehensive data sources are imperative.
# About the Author
**Jiayi Wang**
![](https://miro.medium.com/v2/resize:fit:480/format:webp/1*eZIGDi8LhIzazDbvscYA1Q.png)
Figure 10. Jiayi Wang.

**Jiayi Wang** is a junior student at Duke Kunshan University majoring in Applied Math & Computational Science tracking in Math. He has a solid foundation in Data Science and excels in Math. He has done research in trading strategies and portfolio construction in the Chinese Commodity Market. He is working under the guidance of Prof. Luyao Zhang on machine learning for Blockchain Security and Privacy.
# Acknowledgments
**Interim Executive Editors:** Xintong Wu, Wanglin Deng, Yutong Quan, Colden Johnson

**Associate Editor:** Xinyu Tian

**Chief Editor:** Prof. Luyao Zhang
Design: Yixuan Li