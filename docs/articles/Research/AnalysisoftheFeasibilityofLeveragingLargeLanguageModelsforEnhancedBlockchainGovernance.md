Analysis of the Feasibility of Leveraging Large Language Models for Enhanced Blockchain Governance
====================================================================================

Can we apply large language models to blockchain social governance?
----------------------------------------------------------------------------------

> Disclaimer: “This article is a final deliverable from Prof. Luyao Zhang’s project entitled “From ‘Code is Law’ to ‘Code and Law’: A Comparative Study on Blockchain Governance,” supported by the 2023 Summer Research Scholarship (SRS) program at Duke Kunshan University. Our Summer 2023 scholars also receive additional support from Wang-Cai Biochemistry Lab Donation Fund. SciEcon wholeheartedly supports DKU’s noble mission of advancing interdisciplinary research and fostering integrated talents. Our support is solely focused on promoting academic excellence and knowledge exchange. SciEcon does not seek any financial gains, property rights, or branding privileges from DKU. Moreover, individuals involved in this philanthropy event perform their roles independently at DKU and SciEcon.”

**Keywords(hashtags)**
================

#large language model #natural language processing #blockchain #blockchain governance

**Highlights:**
================
1. Research: Researches mainstream large language models, examines their technical architecture and classification, and explores open-source models. Additionally, the importance of blockchain governance, particularly social governance, is emphasized, along with the introduction of open-source forum discussion data for natural language processing tasks.
2. Innovation: Explores the potential application of large language models to enhance blockchain social governance. By leveraging the capabilities of these models, new insights and approaches can be developed to address the challenges associated with blockchain technologies, particularly from a social perspective.
3. Leadership: Provides valuable guidance on future research frameworks aiming to apply large language models in addressing the unique challenges posed by blockchain technologies. By highlighting the significance of social governance in blockchain networks and promoting the utilization of large language models, this research aims to advance the field and provide leadership in this study area.


**Introduction**
================
As ChatGPT explodes and artificial intelligence (AI) technology continues to evolve, the natural language processing (NLP) technology behind its success, large language models (LLMs), has attracted widespread attention and popularity. LLMs are Transformer language models containing hundreds of billions (or more) of parameters trained on large amounts of unlabeled text data ([Trummer 2023](https://arxiv.org/abs/2306.09339); [Kim and Lee 2023](https://arxiv.org/abs/2305.09620)). Given a sufficiently large number of parameters and training data, LLMs can perform a wide range of tasks with little or no specialized training, including text generation and summarization, question and answer, translation, topic analysis, and sentiment analysis ([Trummer 2023](https://arxiv.org/abs/2306.09339); [Yang et al. 2023](https://arxiv.org/abs/2304.13712); [Zhao et al. 2023](https://arxiv.org/abs/2303.18223); [Ling et al. 2023](https://arxiv.org/abs/2305.18703); [Wang et al. 2023](https://arxiv.org/abs/2301.11916)). LLMs have found applications in diverse domains, including social, natural, and applied sciences, showcasing their accuracy and effectiveness ([Ling et al. 2023](https://arxiv.org/abs/2305.18703)). However, their integration with blockchain technology remains limited, and more research needs to be conducted on leveraging LLMs for blockchain governance.

Blockchain, another disruptive technology alongside AI, enables decentralized economies by establishing trust in peer-to-peer networks ([Zhang et al. 2022](https://arxiv.org/abs/2205.04256)). A robust governance system is essential to ensure the success and sustainability of blockchain platforms ([Laatikainen et al. 2023](https://www.sciencedirect.com/science/article/pii/S0950584923000034#bib0010); [Kiayias and Lazos 2023](https://arxiv.org/abs/2201.07188)). However, the decentralized nature and automation of governance decisions present challenges such as participation levels in voting, unfairness stemming from plutocratic systems, conflicts of interest, and a lack of transparency ([Kiayias and Lazos 2023](https://arxiv.org/abs/2201.07188); [Laatikainen et al. 2023](https://www.sciencedirect.com/science/article/pii/S0950584923000034#bib0010)). In exploring blockchain governance, it is essential to notice the increasing significance of social factors in blockchain governance. Whether for on-chain or off-chain governance, social networks and media activities influence the opinions and decisions of miners and token holders during the voting process ([Laatikainen et al. 2023](https://www.sciencedirect.com/science/article/pii/S0950584923000034#bib0010)). Moreover, studying decentralized communities can uncover the impact of group behavior within informal spaces on decision-making outcomes ([Rennie et al. 2022](https://journals.sagepub.com/doi/10.1177/10778004221097056)).

Considering that the behavior of participants in blockchain communities is mainly described through language, including complaints, questions, and suggestions on social platforms such as blogs and forums ([Rennie et al. 2022](https://journals.sagepub.com/doi/10.1177/10778004221097056)), this article argues LLMs can be a promising tool to deeply explore the discussions and topics within decentralized communities, and ultimately enhance blockchain governance through social means.

This article explores the feasibility of using LLMs to enhance blockchain social governance and decision-making. The article starts with a concise introduction to LLMs and the Transformer architecture, followed by a discussion on classifying Transformer-based language models and algorithmic architectures. Additionally, the article discusses h2oGPT, an open-source repository facilitating the creation and utilization of LLMs, and explores its potential applications in broader AI research.

Another focus of this article is blockchain. For this section, the article initially underscores the significance and categorization of blockchain governance. Subsequently, it emphasizes the necessity of focusing on social governance means to enhance decision-making capabilities. Finally, the article introduces open-source blockchain discussion data from Discord, a prominent blockchain governance communication forum that can train LLMs.


**Large Language Models**
================
Introduction to LLMs and Transformer
------------
Large Language Models (LLMs) are advanced Transformer-based language models with many parameters, often hundreds of billions or even more ([Trummer 2023](https://arxiv.org/abs/2306.09339)). These models are trained on extensive amounts of unlabeled text data, enabling them to exhibit remarkable capabilities in natural language processing (NLP) tasks ([Trummer 2023](https://arxiv.org/abs/2306.09339); [Kim and Lee 2023](https://arxiv.org/abs/2305.09620)). The Transformer architecture, introduced by Vaswani (2016), lies at the heart of the NLP revolution and serves as the dominant framework for various NLP tasks ([Trummer 2023](https://arxiv.org/abs/2306.09339)). It has also found increasing application in computer vision, audio analysis, and multimodal data analysis ([Trummer 2023](https://arxiv.org/abs/2306.09339)).

The main innovation of the Transformer architecture lies in the self-attention mechanism, which facilitates the calculation of the probability of a word appearing in the context of other words ([Strasser 2023](https://arxiv.org/abs/2303.17511)). The mechanism enables highly parallelized operations, thus making it possible to create large-scale language models ([Trummer 2023](https://arxiv.org/abs/2306.09339); [Zhao et al. 2023](https://arxiv.org/abs/2303.18223)). Based on the Transformer architecture, BERT was proposed ([Devlin 2019](https://arxiv.org/abs/1810.04805)). Using a specifically designed pre-training task, BERT leverages pre-training on a vast unlabeled corpus ([Devlin 2019](https://arxiv.org/abs/1810.04805); [Zhao et al. 2023](https://arxiv.org/abs/2303.18223)). The research on BERT sparked extensive research and popularized the “pre-train and fine-tune” learning paradigm, wherein pre-trained context-aware word representations serve as highly effective general semantic features, enhancing the overall performance and generality of NLP tasks ([Zhao et al. 2023](https://arxiv.org/abs/2303.18223)). Fine-tuning, as a complementary step to pre-training, involves providing task-specific instructions to the model. It is typically employed for addressing new tasks not previously encountered during the expansion of the language model ([Trummer 2023](https://arxiv.org/abs/2306.09339)). Following the “pre-train and fine-tune” paradigm, LLMs are developed by further scaling up the model size, increasing the volume of training data, and leveraging significant computational resources ([Zhao et al. 2023](https://arxiv.org/abs/2303.18223)).


Classification of Transformer-based Language Models and Algorithmic Architectures
------------
On April 26, Amazon, in collaboration with researchers from several U.S. universities, released a comprehensive and practical guide for practitioners and end users to use LLMs in downstream NLP tasks ([Yang et al. 2023](https://arxiv.org/abs/2304.13712)). Readers are directed to the [paper](https://arxiv.org/abs/2304.13712), and the associated [GitHub](https://github.com/Mooler0410/LLMsPracticalGuide) repository for more detailed information and additional resources. In this subsection, the technical architecture and model classification of LLMs will be discussed, drawing upon the contributions made by [Yang et al. (2023)](https://arxiv.org/abs/2304.13712).

The current mainstream development of LLMs primarily revolves around the Transformer architecture, which serves as the foundation for language models. LLMs can be categorized into two main types: Encoder-Decoder (or Encoder-only) and Decoder-only models. Fig. 1 illustrates these two algorithmic architectures’ technical characteristics and model representatives.

![](https://miro.medium.com/v2/resize:fit:1400/format:webp/1*DPSr2l_WXKlVSWttHpxuOw.png)<br />Figure 1: Summary of LLMs (cited from [Yang et al. 2023](https://arxiv.org/abs/2304.13712)).

The research paper also employs a visualized tree diagram (see Fig. 2) to summarize the evolution of LLMs. This diagram summarizes the current state-of-the-art of LLMs, encompassing technical architecture and open-source availability.

![](https://miro.medium.com/v2/resize:fit:1400/format:webp/1*gTexZQgXGYDdlgM74DZeAw.jpeg)<br />Figure 2: The evolutionary tree of modern LLMs (cited from [Yang et al. 2023](https://arxiv.org/abs/2304.13712)).

In this diagram, the *pink* branch refers to the Encoder-Only model. The initial rapid growth of this branch was spurred by the release of BERT by Google. However, its growth gradually decelerated after 2020.

The *green* branch represents the Encoder-Decoder model with powerful sequence learning and generation capabilities. This model type is especially good at mapping input sequences to output sequences, making it particularly suitable for translation and text generation tasks.

Finally, the *blue* branch corresponds to the Decoder-Only model. Initially, these models were less popular than the other two types. However, after 2021, Decoder-Only models experienced a significant surge in interest, primarily driven by the introduction of GPT-3. Notably, **OpenAI** has consistently maintained its leading position in the LLM area through the development of GPT-3 and the ongoing advancements with GPT-4, showcasing its strong commitment to pushing the boundaries of this technology.

According to the evaluation of the degree of openness in LLMs, it is widely recognized that Meta has made substantial contributions to the open-source community, particularly in the context of LLMs. Meta’s dedication to open-source principles is evident in their release of all LLMs as open-source. However, despite Meta’s commitment, the overall trend in LLM development shows a growing inclination towards closed-source models.

Before 2020, most LLMs were open-source, allowing for extensive academic research and experimentation. However, with the introduction of GPT-3, there has been a noticeable increase in the number of model sources that have transitioned to closed-source. Conducting research experiments related to LLMs has become more challenging, limiting the accessibility of these models for academic purposes.

As a result, there is a potential shift towards API-based research as the dominant approach in academia, where researchers rely on utilizing LLM models through application programming interfaces (APIs) provided by companies rather than having direct access to the underlying model code. This trend raises concerns about the impact on academic research and the availability of LLMs for scientific exploration.


h2oGPT
------------
Fortunately, introducing h2oGPT ([Candel et al. 2023](https://arxiv.org/abs/2306.08161)) has facilitated broader exploration and advancement in LLMs. h2oGPT encompasses a collection of openly accessible repositories designed for developing and utilizing LLMs based on Generative Pretrained Transformers (GPTs) ([Candel et al. 2023](https://arxiv.org/abs/2306.08161)). To enhance practicality, the researchers have generated various fine-tuned h2oGPT models, granting full permissions under the Apache 2.0 licenses, thereby permitting commercial use. These models can be tailored or expanded based on open-source LLMs to cater to specific requirements at a relatively economical expense. Moreover, h2oGPT can be accessed locally or via a private cloud, guaranteeing uninterrupted availability and reducing reliance on external providers. This platform offers increased flexibility, control, and cost efficiency for subsequent research endeavors while safeguarding data privacy and security.

Subsequently, this subsection delivers a concise overview of the accessible models, utilized data, and operational processes of h2oGPT. Further comprehensive information can be obtained from the [h2oGPT GitHub](https://github.com/h2oai/h2ogpt) and [H2O LLM Studio GitHub](https://github.com/h2oai/h2o-llmstudio#data-format) repositories.

The current (May 2023) available foundation models provided by h2oGPT are:

*1. EleutherAI/pythia-6.9b*

*2. EleutherAI/pythia-12b and EleutherAI/pythia-12b-deduped*

*3. EleutherAI/gpt-neox-20b*

*4. mosaicml/mpt-7b-storywriter*

*5. tiiuae/falcon-7b*

*6. ttiuae/falcon-40b*

*7. bigscience/bloom*

Smaller models, specifically Falcon, which are trained on a more significant number of tokens, have demonstrated superior performance and can accommodate longer context lengths compared to Eleuther AI and bigscience models. Falcon models were trained on the RefinedWeb dataset, comprising 2.8 TiB of Internet data. On the other hand, the Pile dataset, consisting of 825 GiB of data, including some questionable content, was used to train all other models.

The subsequent step in the process is fine-tuning, which causes the preparation of a fine-tuning dataset. This dataset typically includes input (cues) and output (responses). To streamline the model’s learning process, researchers create simple data pairs such as “input”: “Who are you?” and “output”: “I am h2oGPT.” Aside from generating input/output pairs, the fine-tuning dataset incorporates prompt engineering (e.g., injecting <human>: and <bot>: into the text to show input/output), data pre-processing (e.g., removing incomplete sentences and excessively long conversations), and data filtering (e.g., eliminating profanity or inadequate responses that are too short or of poor quality).

To facilitate the preparation of fine-tuned datasets, researchers have developed H2O LLM Data Studio, a toolkit designed explicitly for LLM fine-tuning data preparation. LLM Data Studio supports various downstream tasks, including question answering, text summarization, instruction tuning, human-machine dialogue, and continuous pre-training. It provides 11 essential techniques, including data augmentation, text cleaning, and profanity check to assist users with all aspects of data cleaning and preparation for fine-tuning LLMs.

h2oGPT offers two fine-tuning techniques: LoRA (Low Rank Approximation) and bitsandbytes. LoRA achieves significant speedup and reduces memory usage by training parameters around 0.1% of the original weights. It focuses on fine-tuning specific parts of the neural network architecture, such as attention heads, to prevent catastrophic forgetting. This makes LoRA an effective technique for efficient fine-tuning. To further mitigate the memory requirements of expensive GPU hardware, h2oGPT researchers use bitsandbytes to implement 8-bit basic models for training or inference. This approach reduces memory costs by approximately two times compared to using LoRA alone. Despite the slight decrease in accuracy, the benefits of acceleration and cost savings outweigh the drawbacks.

To ensure the usability of h2oGPT for research purposes, the developers evaluated the model metrics using the EleutherAI evaluation tool. This evaluation confirmed that the fine-tuned LLMs retained the fundamental capabilities of the foundation models.

Given the open-source attributes of h2oGPT and its potential applicability in research, it is conceivable to explore the utilization of fine-tuned LLMs across diverse NLP tasks. Notably, there exists an untapped area within the realm of LLMs where they have yet to be fully integrated, namely blockchain governance. Following the development logic espoused by the h2oGPT researchers makes it possible to investigate the prospects of employing fine-tuned LLMs to facilitate and advance blockchain governance, expanding the current boundaries of LLM applications.

**Blockchain Governance**
================
A Glance into Blockchain Governance
------------
Blockchain is a decentralized ledger system that employs synchronization mechanisms within a peer-to-peer database to enable transaction verification, recording, and distribution without intermediaries, thus eliminating the need to place trust in third parties ([Laatikainen et al. 2023](https://www.sciencedirect.com/science/article/pii/S0950584923000034#bib0010)). This technology leverages smart contracts, which refer to code deployed within a blockchain environment or the source code from which such code is compiled. Additionally, oracles serve as digital interfaces that link external data sources to the blockchain system; In contrast, consensus mechanisms provide fault-tolerant methods for authenticating and validating values or transactions on a distributed ledger, all without the involvement of intermediaries ([Laatikainen et al. 2023](https://www.sciencedirect.com/science/article/pii/S0950584923000034#bib0010)). As blockchain technology matures, its applications have expanded into various domains, such as data sharing, item tracking, supply chain monitoring, power systems, and digital voting ([Mosley et al. 2022](https://journals.sagepub.com/doi/10.1177/107780042210970567/10778004221097056)). By enabling distributed trust, blockchain empowers a decentralized economy ([Zhang et al. 2022](https://arxiv.org/abs/2205.04256)).

The benefits of blockchain are significant, but it is also facing many challenges ([Laatikainen et al. 2023](https://www.sciencedirect.com/science/article/pii/S0950584923000034#bib0010); [Kiayias and Lazos 2023](https://arxiv.org/abs/2201.07188)). As Kai Sedgwick stated,

*“The greatest challenge new blockchains must solve isn’t speed or scaling — it’s governance.”* ([Laatikainen et al. 2023](https://www.sciencedirect.com/science/article/pii/S0950584923000034#bib0010))

Other studies have also highlighted that a robust governance system is essential for successfully developing blockchains and their ability to adapt, evolve and interact ([Laatikainen et al. 2023](https://www.sciencedirect.com/science/article/pii/S0950584923000034#bib0010); [Kiayias and Lazos 2023](https://arxiv.org/abs/2201.07188); [Mosley et al. 2022](https://journals.sagepub.com/doi/10.1177/107780042210970567/10778004221097056)). Suitable governance mechanisms can prevent participants from operating untrustworthy and limit blockchain systems from entering crises ([Laatikainen et al. 2023](https://www.sciencedirect.com/science/article/pii/S0950584923000034#bib0010)). Unlike centralized organizations that a few individuals manage, blockchain platforms are run by different participants in a decentralized manner ([Kiayias and Lazos 2023](https://arxiv.org/abs/2201.07188)). Like other organizations, blockchain platforms try to adapt and adjust to stakeholders’ needs and preferences ([Kiayias and Lazos 2023](https://arxiv.org/abs/2201.07188)). However, based on the decentralized nature, the preferences of different participants may not always coincide, and therefore governance issues arise, including the level of participation in the voting process, unfairness in voting because of plutocratic systems (those with more tokens have more decision-making power); conflict of interest in voting; and lack of transparency ([Kiayias and Lazos 2023](https://arxiv.org/abs/2201.07188); [Laatikainen et al. 2023](https://www.sciencedirect.com/science/article/pii/S0950584923000034#bib0010)). How to address governance issues effectively and exploit the disruptive potential of blockchain deserves great attention.

The existing literature provides a systematic overview of blockchain governance definitions, classifications, and means classifications and means ([Laatikainen et al. 2023](https://www.sciencedirect.com/science/article/pii/S0950584923000034#bib0010); [Kiayias and Lazos 2023](https://arxiv.org/abs/2201.07188); [Mosley et al. 2022](https://journals.sagepub.com/doi/10.1177/107780042210970567/10778004221097056)). In a broad context, governance entails regulating the decision-making processes among participants to achieve common objectives that contribute to the development, reinforcement, or perpetuation of social norms and institutions ([Laatikainen et al. 2023](https://www.sciencedirect.com/science/article/pii/S0950584923000034#bib0010)). While researchers have not established a specific definition of governance within the blockchain domain, various classifications exist ([Laatikainen et al. 2023](https://www.sciencedirect.com/science/article/pii/S0950584923000034#bib0010)). Firstly, *governance of the infrastructure* encompasses the means and processes involved in directing, controlling, and coordinating participants within a blockchain system. On the other hand, *governance by the infrastructure* refers to the utilization of blockchain to govern actions and behaviors ([Laatikainen et al. 2023](https://www.sciencedirect.com/science/article/pii/S0950584923000034#bib0010)). Secondly, *on-chain governance* pertains to the encoding of rules and decision processes directly into the blockchain system, whereas *off-chain governance* refers to the non-technical rules and decision processes that impact the development and operation of the blockchain system ([Laatikainen et al. 2023](https://www.sciencedirect.com/science/article/pii/S0950584923000034#bib0010)). Thirdly, *technology governance* involves overseeing the technological development of the blockchain system, while *network governance* focuses on the governance of the associated blockchain network ([Laatikainen et al. 2023](https://www.sciencedirect.com/science/article/pii/S0950584923000034#bib0010)). Lastly, *external governance* involves decisions made outside the blockchain system that affect management decisions, while *internal governance* encompasses the governance practices carried out within the system ([Laatikainen et al. 2023](https://www.sciencedirect.com/science/article/pii/S0950584923000034#bib0010)).

Governance encompasses the actions, systems, methods, and processes that facilitate decision-making and can be broadly categorized into technical and social means (Laatikainen et al., 2023). Technical means primarily serve on-chain governance and automate governance decisions through various voting mechanisms, such as smart contracts, DApp frameworks, and consensus algorithms ([Laatikainen et al. 2023](https://www.sciencedirect.com/science/article/pii/S0950584923000034#bib0010)). However, it is essential to note that technical means alone cannot bear the responsibility of governance decisions, as off-chain governance also causes the involvement of social means ([Laatikainen et al. 2023](https://www.sciencedirect.com/science/article/pii/S0950584923000034#bib0010)).

Social governance emphasizes formal and informal communication and collaboration among actors, such as discussions conducted through forums and informal online voting on decisions ([Laatikainen et al. 2023](https://www.sciencedirect.com/science/article/pii/S0950584923000034#bib0010)). Additionally, social media acts as an information broker and influences critical stakeholders in blockchain governance ([Laatikainen et al. 2023](https://www.sciencedirect.com/science/article/pii/S0950584923000034#bib0010)).


Why Social Governance?
------------
Early research has delved into various strategies for optimizing blockchain governance. For example, one approach involves enhancing the voting mechanism by implementing quadratic voting ([Kiayias and Lazos 2023](https://arxiv.org/abs/2201.07188)). In this mechanism, the cost of casting votes follows a quadratic pattern, whereby the cost of 2 votes is 4, and so on ([Kiayias and Lazos 2023](https://arxiv.org/abs/2201.07188)). This approach aims to strike a better balance between Token-Based Suffrage and Identity-Based Suffrage, thereby mitigating the risk of plutocratic politics, where individuals with more token holdings wield greater decision-making power ([Kiayias and Lazos 2023](https://arxiv.org/abs/2201.07188)). By adopting quadratic voting, governance fairness can be upheld.

However, it is worth noting that our study acknowledges the growing significance of social factors, specifically public discourse, within blockchain governance. For instance, [Filippi and Loveluck (2016)](https://hal.science/hal-01382007) extensively examined blockchain governance structures. They concluded that more than technology alone could be needed to address most of the social and political challenges encountered in blockchain networks. [Kiayias and Lazos (2023)](https://arxiv.org/abs/2201.07188) observed that many blockchains combine on-chain governance with off-chain elements, using forum discussions as part of a formal governance model. Moreover, [Rennie et al. (2022)](https://journals.sagepub.com/doi/10.1177/10778004221097056) conducted an ethnographic study of governance interactions within blockchain forums, uncovering how activities in decentralized communities’ informal spaces influence decision outcomes. Consequently, this article argues that a comprehensive exploration of the social dimensions of blockchain governance is warranted. Specifically, it encourages investigation of how suggestions, debates, and complaints put forth by participants and the broader public on voting platforms, as well as open communication regarding system design on public media (such as blog posts, social channels, podcasts, etc.), can contribute to enhancing decision-making processes and governance.


Available Forum Discussion Data
------------
An extensive literature review has identified several potential sources of blockchain social discussion data, including Discord, Twitter, Reddit, Slack, and Github. Among these, we propose utilizing discussion data from Discord, a popular communication platform for discussing blockchain governance, as a dataset for analyzing blockchain social governance. To obtain Discord chat data, we can utilize [DiscordChatExporter](https://github.com/Tyrrrz/DiscordChatExporter). The resulting data can then be pre-processed using [Clean-Discord](https://github.com/JEF1056/clean-discord) to prepare it for natural language processing tasks.

As previously mentioned, h2oGPT’s open-source large language models have proven effective in various NLP tasks ([Candel et al. 2023](https://arxiv.org/abs/2306.08161)). Therefore, we aim to leverage these models for analyzing the discussion data within blockchain forums. Following the guidelines provided by the h2oGPT developers, we can adapt the Discord data into a fine-tuning dataset, which involves creating input/output data pairs and other necessary preparations. Subsequently, fine-tuning techniques can apply to these open-source models, enabling a more comprehensive analysis of public discourse within the blockchain domain.

By employing various NLP tasks such as text summarization, topic analysis, and sentiment analysis, we can gain valuable insights into the focal points of discussions within the informal spaces of blockchain communities, uncovering overlooked topics and understanding public attitudes toward governance decisions. The application of LLMs will enhance blockchain governance in two significant ways. First, they can help synthesize and analyze the textual content of these discussions, contributing to more inclusive and diverse decision-making processes. Secondly, integrating LLMs can enhance blockchain governance’s transparency by explaining and justifying decisions and policies.


**Conclusion**
================
In conclusion, this article first introduces Large Language Models and provides available open-source models. Additionally, the article discusses the significance of blockchain governance, particularly social governance, and the available forum discussion data. Through an examination of the extensive literature and resources, using LLMs can enhance the decision-making process of blockchain governance while promoting transparency and inclusiveness. However, it is essential to note that further empirical research is required to validate the feasibility and effectiveness of this proposal.


**Relevant Materials**
================

\[1\] Candel, A., McKinney, J., Singer, P., Pfeiffer, P., Jeblick, M., Prabhu, P., Gambera, J., Landry, M., Bansal, S., Chesler, R., Lee, C.M., Conde, M.V., Stetsenko, P., Grellier, O. and Ambati, S. (2023). *h2oGPT: Democratizing Large Language Models.* [online] arXiv.org. doi:https://doi.org/10.48550/arXiv.2306.08161.

\[2\] Devlin, J., Chang, M.-W., Lee, K. and Toutanova, K. (2018). *BERT: Pre-training of Deep Bidirectional Transformers for Language Understanding.* [online] arXiv.org. Available at: https://arxiv.org/abs/1810.04805.

\[3\] Fan, J.E. (2023). *Clean-Discord.* [online] GitHub. Available at: https://github.com/JEF1056/clean-discord [Accessed 19 Jun. 2023].

\[4\] Filippi, P. de and Loveluck, B. (2016). The invisible politics of Bitcoin: governance crisis of a decentralised infrastructure. *Internet Policy Review.* [online] Available at: https://hal.science/hal-01382007 [Accessed 19 Jun. 2023].

\[5\] “H2oai/H2o-Llmstudio.” *GitHub*, 19 June 2023, github.com/h2oai/h2o-llmstudio#data-format. Accessed 19 June 2023.

\[6\] “H2oai/H2ogpt.” *GitHub*, 19 June 2023, github.com/h2oai/h2ogpt. Accessed 19 June 2023.

\[7\] Holub, O. (2022). *DiscordChatExporter.* [online] GitHub. Available at: https://github.com/Tyrrrz/DiscordChatExporter.

\[8\] Kiayias, A. and Lazos, P. (2022). SoK: Blockchain Governance. *arXiv:2201.07188 [cs]*. [online] Available at: https://arxiv.org/abs/2201.07188.

\[9\] Kim, Junsol, and Byungkyu Lee. “AI-Augmented Surveys: Leveraging Large Language Models for Opinion Prediction in Nationally Representative Surveys.” *ArXiv.org*, 16 May 2023, arxiv.org/abs/2305.09620. Accessed 20 June 2023.

\[10\] Laatikainen, G., Li, M. and Abrahamsson, P. (2023). A system-based view of blockchain governance. *Information and Software Technology*, 157, p.107149. doi:https://doi.org/10.1016/j.infsof.2023.107149.

\[11\] Ling, C., Zhao, X., Lu, J., Deng, C., Zheng, C., Wang, J., Chowdhury, T., Li, Y., Cui, H., Zhang, X., Zhao, T., Panalkar, A., Cheng, W., Wang, H., Liu, Y., Chen, Z., Chen, H., White, C., Gu, Q. and Yang, C. (2023). *Beyond One-Model-Fits-All: A Survey of Domain Specialization for Large Language Models.* [online] arXiv.org. doi:https://doi.org/10.48550/arXiv.2305.18703.

\[12\] Mooler0410. “The Practical Guides for Large Language Models.” *GitHub*, 19 June 2023, github.com/Mooler0410/LLMsPracticalGuide. Accessed 19 June 2023.

\[13\] Mosley, L., Pham, H., Guo, X., Bansal, Y., Hare, E. and Antony, N. (2022). Towards a systematic understanding of blockchain governance in proposal voting: A dash case study. *Blockchain: Research and Applications*, p.100085. doi:https://doi.org/10.1016/j.bcra.2022.100085.

\[14\] Rennie, E., Zargham, M., Tan, J., Miller, L., Abbott, J., Nabben, K. and De Filippi, P. (2022). Toward a Participatory Digital Ethnography of Blockchain Governance. *Qualitative Inquiry*, p.107780042210970. doi:https://doi.org/10.1177/10778004221097056.

\[15\] Strasser, A. (2023). On pitfalls (and advantages) of sophisticated large language models. *arXiv:2303.17511 [cs]*. [online] Available at: https://arxiv.org/abs/2303.17511.

\[16\] Trummer, I. (2022). From BERT to GPT-3 codex. *Proceedings of the VLDB Endowment*, 15(12), pp.3770–3773. doi:https://doi.org/10.14778/3554821.3554896.

\[17\] Vaswani, A., Shazeer, N., Parmar, N., Uszkoreit, J., Jones, L., Gomez, A.N., Kaiser, L. and Polosukhin, I. (2017). *Attention Is All You Need*. [online] arXiv.org. Available at: https://arxiv.org/abs/1706.03762.

\[18\] Wang, X., Zhu, W., Saxon, M., Steyvers, M. and Wang, W.Y. (2023). *Large Language Models Are Implicitly Topic Models: Explaining and Finding Good Demonstrations for In-Context Learning.* [online] arXiv.org. doi:https://doi.org/10.48550/arXiv.2301.11916.

\[19\] Yang, J., Jin, H., Tang, R., Han, X., Feng, Q., Jiang, H., Yin, B. and Hu, X. (2023). Harnessing the Power of LLMs in Practice: A Survey on ChatGPT and Beyond. doi:https://doi.org/10.48550/arxiv.2304.13712.

\[20\] Zhang, L., Ma, X. and Liu, Y. (2022). SoK: Blockchain Decentralization. *arXiv:2205.04256 [cs, econ, q-fin]*. [online] Available at: https://arxiv.org/abs/2205.04256.

\[21\] Zhao, W.X., Zhou, K., Li, J., Tang, T., Wang, X., Hou, Y., Min, Y., Zhang, B., Zhang, J., Dong, Z., Du, Y., Yang, C., Chen, Y., Chen, Z., Jiang, J., Ren, R., Li, Y., Tang, X., Liu, Z. and Liu, P. (2023). A Survey of Large Language Models. *arXiv:2303.18223 [cs].* [online] Available at: https://arxiv.org/abs/2303.18223.


**About the Author**
================
**Yutong Quan**

![](https://miro.medium.com/v2/resize:fit:608/format:webp/1*G4XrJDMve4AA4c_A0GtqzA.png)<br />Figure 3: Yutong Quan.

*Yutong Quan* is a student at Duke Kunshan University, Class of 2024, majoring in Political Economy with an Economics track. Interested research areas include blockchain governance, decentralized finance, and interdisciplinary fields of Artificial Intelligence and economics.

Please contact her at *yutongq@outlook.com*.

**Acknowledgments**
================
My sincere appreciation to SciEcon Insights and its directors:

**Interim Executive Editors**: Xintong Wu, Wanlin Deng

**Associate Editor**: Xinyu Tian

**Chief Editor**: Prof. Luyao Zhang

**Design**: Yixuan Li
