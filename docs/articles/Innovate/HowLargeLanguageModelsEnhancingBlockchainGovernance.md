How Large Language Models Enhancing Blockchain Governance
====================================================================================

Data and Methods Overview
----------------------------------------------------------------------------------

> Disclaimer: “This article is a final deliverable from Prof. Luyao Zhang’s project entitled “From ‘Code is Law’ to ‘Code and Law’: A Comparative Study on Blockchain Governance,” supported by the 2023 Summer Research Scholarship (SRS) program at Duke Kunshan University. Our Summer 2023 scholars also receive additional support from Wang-Cai Biochemistry Lab Donation Fund. SciEcon wholeheartedly supports DKU’s noble mission of advancing interdisciplinary research and fostering integrated talents. Our support is solely focused on promoting academic excellence and knowledge exchange. SciEcon does not seek any financial gains, property rights, or branding privileges from DKU. Moreover, individuals involved in this philanthropy event perform their roles independently at DKU and SciEcon.”

**Keywords(hashtags)**
================

#large language models #blockchain governance #discord #h2ogpt #uniswap

**Supplementary Code**
================

The supplementary code of this article is released as open source on GitHub: https://github.com/SciEcon/SRS2023_LLMs-BlockchainGovernance.

**Highlights:**
================
1. Research: Focus on extracting data from the Uniswap Discord community discussions and explore the integration of H2O.ai’s large language model ecosystem and methodologies.
2. Innovation: Combine the dataset from blockchain forum discussions with natural language processing research methods to gain valuable insights for blockchain governance analysis.
3. Leadership: Lead in driving the adoption of large language models for blockchain governance. The comprehensive tools and platforms empower researchers, practitioners, and decision-makers to utilize data-driven insights in the governance practices of blockchain communities. Foster transparency, inclusivity, and informed decision-making, leading to the evolution and innovation of blockchain governance practices.

![](https://miro.medium.com/v2/resize:fit:1400/format:webp/1*UiCVGomGgty0C1HM0FxZdg.png)<br />Figure. 1: Article Mind Map (created by Whimsical).

**Introduction**
================
In recent years, the deployment of Large Language Models (LLMs) has expanded across various domains, including finance, medicine, and law ([Ling et al. 2023](https://arxiv.org/abs/2305.18703)). LLMs have proven effective in tasks such as text generation and summarization, question answering, translation, topic analysis, and sentiment analysis ([Trummer 2023](https://arxiv.org/abs/2306.09339); [Yang et al. 2023](https://arxiv.org/abs/2304.13712); [Zhao et al. 2023](https://arxiv.org/abs/2303.18223); [Ling et al. 2023](https://arxiv.org/abs/2305.18703); [Wang et al. 2023](https://arxiv.org/abs/2301.11916)). Unlike traditional Natural Language Processing (NLP) models, LLMs leverage large parameters, extensive training data, and substantial computing power to perform these tasks with minimal or no specialized training ([Zhao et al. 2023](https://arxiv.org/abs/2303.18223)).

The combination of LLMs and blockchain is still in its early stages, but the research conducted by [Gai et al. (2023)](https://arxiv.org/pdf/2304.12749.pdf) has made significant contributions to the interdisciplinary field. They introduced a dynamic, real-time method that utilizes LLMs to detect anomalous blockchain transactions. This approach offers several advantages, including an expansive search space and the ability to detect a broader spectrum of anomalies without depending on pre-defined rules or patterns. The proposed tool, BLOCKGPT, generates trace representations of blockchain activity and trains a large language model from scratch to serve as a real-time Intrusion Detection System. These contributions enhance blockchain security and have positive implications for the future development of decentralized systems.

Existing literature has primarily focused on utilizing LLMs to detect anomalous blockchain transactions. In contrast, our research is dedicated to exploring the potential of LLMs in enhancing social governance within blockchain networks. Through our previous [literature review](/articles/Innovate/how-blockchain-empowers-market-design-rules-and-data.html), we have identified the significant potential of LLMs in enhancing social governance within blockchain networks. LLMs can facilitate a more inclusive and diverse decision-making process by synthesizing and analyzing textual discussions within blockchain communities. Furthermore, LLMs can contribute to the transparency of blockchain governance by providing explanations and justifications for decisions made.

The article aims to introduce two main components. Firstly, we will present a dataset of discussions from the Uniswap community on the Discord forum. This dataset will serve as a valuable resource for training and evaluating LLMs in the context of blockchain governance. Secondly, we will demonstrate an application method utilizing h2oGPT, an open-source repository of LLMs, to apply these models to blockchain social governance.


**Data: Discord**
================
[Discord](https://discord.com/) is a popular public communication forum where various topics, including blockchain communities, are frequently discussed. In the realm of cryptocurrencies, these communities’ social structure and organizational psychology hold equal importance to formal voting systems. The Discord server has emerged as a practical space for individuals to familiarize themselves with protocols, engage with community members, and explore opportunities for active participation within the network. Ideally, proposals and ideas evolve through conversations and debates in Discord chats, often leading to constructive disagreements. Informal communication channels such as these are vital in fostering engagement and participation within the crypto community.

Among the various on-chain governance protocol communities, the [Uniswap](https://uniswap.org/) community stands out as one of the largest. Uniswap possesses a well-constructed [Discord](https://discord.com/) channel where users and stakeholders congregate for conversations and support. One channel, *#governance* on Uniswap Discord, serves as the hub for discussions on how Uniswap should evolve (Fig. 2). Most activities in the *#governance* channel revolve around inquiries about the governance process and grievances regarding unfavorable decisions made by the core team and representatives.

![](https://miro.medium.com/v2/resize:fit:1400/format:webp/1*Rg02ncB8lY2WYWhoklg5xQ.png)<br />Figure. 2: Screenshot of Uniswap Discord #governance channel.

To collect data from the discussions on the Uniswap Discord *#governance* channel, we utilized the DiscordChatExporter tool (Fig. 3). For more information about DiscordChatExporter, please refer to https://github.com/Tyrrrz/DiscordChatExporter.

![](https://miro.medium.com/v2/resize:fit:1400/format:webp/1*Cct3IJvb__9Onr6lR_luaA.png)<br />Figure. 3: DiscordChatExporter Application.

DiscordChatExporter allows us to easily access all the discussion data since the channel’s inception. Our dataset comprises a total of 11,549 discussions within the Uniswap *#governance* channel, spanning from September 17, 2020 (the first discussion) to the morning of June 28, 2023 (Fig. 4). The dataset includes variables such as AuthorID, Author, Date, Content, Attachment, and Reactions.

![](https://miro.medium.com/v2/resize:fit:1400/format:webp/1*VIoTEpuKM4duLZI1a8Cwcg.png)<br />Figure. 4: Uniswap Discord #governance channel discussion dataset.

Furthermore, we conducted a preliminary visualization of the dataset. Fig. 5 illustrates a time series plot depicting the volume of discussions in the Uniswap *#governance* channel. In the early stages of the channel’s creation in 2020, there was a relatively high discussion surrounding Uniswap community governance. However, in the subsequent three years, the volume of discussions remained relatively low.

![](https://miro.medium.com/v2/resize:fit:1400/format:webp/1*zGSxJGsaT_bVUrgMSL5_Tg.png)<br />Figure. 5: Uniswap Discord #governance channel discussion volume.

Additionally, Fig. 6 shows a word cloud diagram generated from the forum discussions. The keywords predominantly revolve around two main aspects: Uniswap (e.g., uniswap, uni) and blockchain governance (e.g., governance, proposal, vote).

![](https://miro.medium.com/v2/resize:fit:1400/format:webp/1*payuidq__-MHq2urLV7eIg.png)<br />Figure. 6: Word cloud of uniswap Discord #governance channel discussions.

However, the above analysis provides only a general overview of the dataset. Our study will conduct a further in-depth analysis using a large language model regarding the variations in discussion volume and the topics discussed.


**Methods: H2O.ai**
================
The [H2O.ai](https://h2o.ai/) LLM ecosystem offers a comprehensive solution for training large language models using our datasets.

[H2O LLM Data Studio](https://h2o.ai/blog/streamlining-data-preparation-for-fine-tuning-of-large-language-models/) is a code-free data science workbench designed for data preparation in tasks related to LLMs. With its user-friendly web interface (Fig. 7), users can efficiently process tasks such as text cleaning, quality detection, word tokenization, truncation, and reinforcement learning with human feedback (RLHF). Users can then seamlessly utilize the processed data for subsequent tasks like model fine-tuning, further pre-training, text summarization, human-machine dialogue, and instruction adjustment.

![](https://miro.medium.com/v2/resize:fit:1400/format:webp/1*eAQ1w-2CfGOoRJimOV2FlQ.png)<br />Figure. 7: H2O LLM Data Studio web interface (cited from [H2O.ai](https://h2o.ai/blog/streamlining-data-preparation-for-fine-tuning-of-large-language-models/)).

H2O LLM Studio is an integrated development environment (IDE) [1] provided by H2O.ai. H2O LLM Studio offers a graphical user interface (GUI) [2] for fine-tuning state-of-the-art large-scale language models. Fig. 8 illustrates an example of LLM fine-tuning. Starting with a foundation model trained on large autoregressive datasets, we can adapt the LLM more precisely to a specific domain by training the model on pre-processed data. For a detailed guide on using H2O LLM Studio, please visit the official GitHub repository at https://github.com/h2oai/h2o-llmstudio.

![](https://miro.medium.com/v2/resize:fit:1400/format:webp/1*kZvN1ozsFeM2K9MXG6GyJw.png)<br />Figure. 8: H2O LLM Studio fine-tune example (cited from [H2O.ai](https://h2o.ai/blog/effortless-fine-tuning-of-large-language-models-with-open-source-h2o-llm-studio/)).

Before getting started, users need to ensure meeting the following requirements:

*Ubuntu 16.04+ machine with at least one recent Nvidia GPU*

*Nvidia driver version >= 470.57.02*

*At least 24GB of GPU memory for larger models*

*Python 3.10 installed on the computer*

Once the setup is complete, users can access the H2O LLM Studio GUI. Fig. 9 outlines the steps for training the model. First, the dataset needs to be imported in the appropriate format (CSV, zip, or Parquet), and then the experiment can be started within the GUI. It is essential to adjust the model parameters according to the specific requirements of the experiment. Additionally, the platform allows real-time tracking and monitoring of training progress and model performance. After completing the experiments, users can leverage the “Compare experiments” feature to analyze how different model parameters affect performance, ensuring that the fine-tuned model meets the desired metrics. The trained models can be shared with a broader audience through popular machine-learning platforms.

![](https://miro.medium.com/v2/resize:fit:1400/format:webp/1*ED31nvm4CqQhAvo-3WdjAg.png)<br />Figure. 9: H2O LLM Studio experiment steps (cited from [H2O.ai](https://h2o.ai/blog/effortless-fine-tuning-of-large-language-models-with-open-source-h2o-llm-studio/)).

Lastly, we introduce h2oGPT, an open-source repository that provides natural language processing capabilities based on large language models. Built on the GPT architecture, h2oGPT offers pre-trained models and features for text generation, question answering, sentiment analysis, and more. Please refer to the official GitHub repository at https://github.com/h2oai/h2ogpt for specific installation guidelines.

![](https://miro.medium.com/v2/resize:fit:1400/format:webp/1*9SNxDh1MqgdIz4LjUDgk3g.png)<br />Figure. 10: h2oGPT web interface (cited from [H2O.ai](https://github.com/h2oai/h2ogpt)).

Fig. 10 shows an interactive interface for h2oGPT, allowing users to import the original dataset and issue various commands such as “What are some ongoing debates and challenges in the Uniswap governance discussions on Discord?” and “What are the main concerns raised by the Uniswap community regarding governance decisions?”. h2oGPT generates answers by summarizing the Discord discussion text, providing insights for optimizing governance and decision-making processes.

**Conclusion & Discussion**
================
H2O.ai is a robust open-source ecosystem for large language models. Users can accomplish a wide range of NLP tasks by combining data analysis, fine-tuning with H2O LLM Studio, and leveraging the h2oGPT repository. Researchers and practitioners can extract insights from the Uniswap governance discussions by integrating open-source Discord discussion data. H2oGPT can generate answers and contribute to decision-making and governance optimization by asking relevant questions, such as ongoing debates or community concerns.

In conclusion, combining the H2O.ai ecosystem with blockchain forum discussion data unleashes the potential of LLMs to enhance blockchain governance. These tools and methods provide valuable insights, support decision-making, and contribute to the establishment of a more inclusive and transparent blockchain ecosystem.


**Relevant Materials**
================

\[1\] **Integrated development environment (IDE)**

An integrated development environment (IDE) is a software application that provides software developers with a diverse set of tools. These tools commonly include a source code editor, automation tools for building processes, and a debugger. In some cases, IDEs also incorporate compilers and interpreters. Additional features, such as version control systems or other tools, may be integrated to facilitate the development of graphical user interfaces (GUIs). Many modern IDEs also offer class browsers, object browsers, and class hierarchies to aid in the creation of object-oriented software.

[[Wikipedia — Integrated development environment](https://en.wikipedia.org/wiki/Integrated_development_environment)]

\[2\] **Graphical user interface (GUI)**

The graphical user interface (GUI) is a type of user interface that enables users to interact with electronic devices using graphical icons and audio cues instead of relying on text-based interfaces, typed commands, or text-based navigation.

[[Wikipedia — Graphical user interface](https://en.wikipedia.org/wiki/Graphical_user_interface)]

Data Source
----------------
Uniswap Discord: https://discord.com/channels/597638925346930701/755969053280960533

Code Source
----------------
DiscordChatExporter GitHub: https://github.com/Tyrrrz/DiscordChatExporter

h2oGPT GitHub: https://github.com/h2oai/h2ogpt

H2O LLM Studio: https://github.com/h2oai/h2o-llmstudio

Articles
----------------
H2O.ai. 2023a. “Effortless Fine-Tuning of Large Language Models with Open-Source H2O LLM Studio.” H2O.ai. May 1, 2023. https://h2o.ai/blog/effortless-fine-tuning-of-large-language-models-with-open-source-h2o-llm-studio/.

H2O.ai. 2023b. “Streamlining Data Preparation for Fine Tuning of Large Language Models.” H2O.ai. June 14, 2023. https://h2o.ai/blog/streamlining-data-preparation-for-fine-tuning-of-large-language-models/.


**About the Author**
================
**Yutong Quan**

![](https://miro.medium.com/v2/resize:fit:608/format:webp/1*G4XrJDMve4AA4c_A0GtqzA.png)<br />Figure 11: Yutong Quan.

*Yutong Quan* is a student at Duke Kunshan University, Class of 2024, majoring in Political Economy with an Economics track. Interested research areas include blockchain governance, decentralized finance, and interdisciplinary fields of Artificial Intelligence and economics.

Please contact her at *yutongq@outlook.com*.

**Acknowledgments**
================
My sincere appreciation to SciEcon Insights and its directors:

**Interim Executive Editors**: Xintong Wu, Wanlin Deng

**Associate Editor**: Xinyu Tian

**Chief Editor**: Prof. Luyao Zhang

**Design**: Yixuan Li
