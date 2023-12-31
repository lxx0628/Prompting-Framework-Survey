# 🦊 Prompting-Framework-Survey 

A curated list of awesome publications and researchers on prompting framework updated and maintained by [The Intelligent System Security (IS2)](https://is2lab.github.io/).

<div align="center">
  <img src="https://github.com/lxx0628/Prompting-Framework-Survey/blob/main/figure/timeline.png" alt="timeline" width="650" />
</div>


Large language models (LLMs) have made significant advancements in both academia and industry, bringing about a fundamental engineering paradigm shift in many areas. While LLMs are powerful, it is also crucial to best use their power where "prompt"🔧 plays a core role. However, the booming LLMs themselves, including excellent APIs like ChatGPT, have several inherent limitations: 1) temporal lag of training data, and 2) the lack of physical capabilities to perform external actions. 

Recently, we have observed the trend of utilizing prompt-based tools to better utilize the power of LLMs for downstream tasks, but a lack of systematic literature and standardized terminology, partly due to the rapid evolution of this field. Therefore, we survey related prompting tools and promote the concept of the 🌟 "**Prompting Framework**" (PF) 🌟, i.e. the framework for managing, simplifying, and facilitating interaction with large language models. We define the **lifecycle** of the PF as a hierarchical structure, from bottom to top, namely: Data Level, Base Level, Execute Level, and Service Level.

<div align="center">
  <img src="https://github.com/lxx0628/Prompting-Framework-Survey/blob/main/figure/workflow.png" alt="workflow" width="650" />
</div>

We also systematically depict the overall landscape of the emerging PF field and discuss potential future research and challenges. To continuously track the developments in this area, we maintain this repo, which can be a useful resource sharing platform for both academic and industry in this field. 



## 🥜 In a Nutshell

<div align="center">
  <img src="https://github.com/lxx0628/Prompting-Framework-Survey/blob/main/figure/nutshell.png" alt="nutshell" width="450" />
</div>

Prompting Framework is a framework for managing, simplifying, and facilitating interaction with large language models, which adheres to four essential properties: modularity, abstraction, extensibility, and standardization. We define the lifecycle of the PF as a hierarchical structure, from bottom to top, namely: Data Level, Base Level, Execute Level, and Service Level.



**📄 Paper Link**: [Prompting Frameworks for Large Language Models: A Survey](https://arxiv.org/abs/2311.12785)


Looking forward to your attention and lively discussion！ 

Sincerely welcome:

🙋‍♂️ Share good prompting frameworks with us!!!

🙋‍♀️ Share your experience of using different prompting frameworks and your urgent needs and services!!!

🙋 Brainstorm the future shape of prompting frameworks!!!

and more ...

**📮 Contact Details**: liuxiaoxia@zju.edu.cn

## 🦄 Update Log

🎬 【2023.11.21】First version of "Prompting Frameworks for Large Language Models: A Survey" published on arXiv!

## 📖 Table of Content
  - 🔅 [Related Resource](#Related-Resource)
    * [Tools for Exploring Relevant Literature](#Tools-for-Exploring-Relevant-Literature)
    * [Related Survey](#Related-Survey)
  - 🔅 [State-of-the-art Prompting Frameworks](#State-of-the-art-Prompting-Frameworks)
    * [The Shell of LLMs (LLM-SH)](#The-Shell-of-LLMs-(LLM-SH))
    * [Language for Interaction with LLMs (LLM-LNG)](#Language-for-Interaction-with-LLMs)
    * [Output Restrictors of LLMs (LLM-RSTR)](#Output-Restrictors-of-LLMs)
  - 🔅 [Comparative Analysis of Prompting Frameworks](#Comparative-analysis-of-Prompting-Frameworks)
  - 🔅 [Key Components of Prompting Frameworks](#Key-Components-of-Prompting-Frameworks)

### 🌟 Related Resource

Fingers crossed these awesome resources sprinkle some extra magic on your tasks too! 

#### 💼 Tools for Exploring Relevant Literature

| 🐾 Tool | 🌱 Description | 
  |:--------:|:--------:|
  | [Trending Papers](https://trendingpapers.com)   |  A useful tool to help us researchers find and explore papers worth reading first. |
  | [Connected Papers](https://www.connectedpapers.com)   |  Explore academic papers in a visual graph. |

#### 💼 Related Survey

* [A Survey of Large Language Models](https://arxiv.org/abs/2303.18223)
* [A Survey on Large Language Model based Autonomous Agents](https://arxiv.org/abs/2308.11432)


### 🔅 State-of-the-art Prompting Frameworks

Taking into consideration the technical features, design objectives, and application scenarios, the current prompting framework can be broadly covered by three types: The Shell of LLMs (LLM-SH), Language for Interaction with LLMs (LLM-LNG), and Output Restrictors of LLMs (LLM-RSTR). The rationale behind designing the prompting framework is to facilitate the interaction between LLMs and the external world, and different types of prompting frameworks manifest this enhancement effect from different perspectives. 

#### 🧩 The Shell of LLMs

LLM-SH functions are much like a shell or interface layer in computer systems, emphasizing interaction with LLMs by facilitating their engagement with highly capable third parties, thereby enabling stronger interaction between LLMs, users, and external models.

* 🤖 Universal LLM-SH
  | 🦊 Prompting Framework   | 🧚‍♂️ Subcategory | 🔍 Introduction|
  |:--------:|:-------:|:--------|
  | [Haystack](https://github.com/deepset-ai/haystack)   | Universal LLM-SH   | LLM orchestration framework to build customizable, production-ready LLM applications. Connect components (models, vector DBs, file converters) to pipelines or agents that can interact with your data. With advanced retrieval methods, it's best suited for building RAG, question answering, semantic search or conversational agent chatbots. |
  | [Semantic Kernel](https://github.com/microsoft/semantic-kernel)   | Universal LLM-SH   | Integrate cutting-edge LLM technology quickly and easily into your apps.|
  | [Langchain](https://github.com/langchain-ai/langchain)   | Universal LLM-SH   | Building applications with LLMs through composability.|
  | [Griptape](https://github.com/griptape-ai/griptape)   | Universal LLM-SH   | Modular Python framework for AI agents and workflows with chain-of-thought reasoning, tools, and memory. Griptape is an enterprise grade alternative to LangChain.|
  | [PromptFlow](https://github.com/microsoft/promptflow)   | Universal LLM-SH   | Build high-quality LLM apps - from prototyping, testing to production deployment and monitoring.|
  | [LLM-chain](https://github.com/sobelio/llm-chain)   | Universal LLM-SH   | A powerful rust crate for building chains in large language models allowing you to summarise text and complete complex tasks.|
  | [LinGoose](https://github.com/henomis/lingoose)   | Universal LLM-SH   | LinGoose it's a Go framework for developing LLMs-based application using pipelines.|
  | [LLMStack](https://github.com/trypromptly/LLMStack)   | Universal LLM-SH   | No-code platform to build generative AI apps, chatbots and agents with your data.|
  | [OpenDAN](https://github.com/fiatrete/OpenDAN-Personal-AI-OS)   | Universal LLM-SH   | OpenDAN is an open source Personal AI OS , which consolidates various AI modules in one place for your personal use.|
  | [Hyv](https://github.com/failfa-st/hyv)   | Universal LLM-SH   | Chaining AI & API agents to streamline software development and achieve goals collaboratively.|

* 🤖 Domain-Specific LLM-SH
  | 🦊 Prompting Framework   | 🧚‍♂️ Subcategory | 🔍 Introduction|
  |:--------:|:-------:|:--------|
  | [LlamaIndex](https://github.com/run-llama/llama_index)   | Domain-Specific LLM-SH   | LlamaIndex (formerly GPT Index) is a data framework for your LLM applications. |
  | [Embedchain](https://github.com/embedchain/embedchain)   | Domain-Specific LLM-SH   | Data platform for LLMs - Load, index, retrieve and sync any unstructured data.|
  | [AgentVerse](https://github.com/OpenBMB/AgentVerse)   | Domain-Specific LLM-SH   | AgentVerse is designed to facilitate the deployment of multiple LLM-based agents in various applications, which primarily provides two frameworks: task-solving and simulation.|
  | [SuperAGI](https://github.com/TransformerOptimus/SuperAGI)   | Domain-Specific LLM-SH   | A dev-first open source autonomous AI agent framework. Enabling developers to build, manage & run useful autonomous agents quickly and reliably.|
  | [Txtai](https://github.com/neuml/txtai)   | Domain-Specific LLM-SH   | All-in-one open-source embeddings database for semantic search, LLM orchestration and language model workflows.|
  | [AutoChain](https://github.com/Forethought-Technologies/AutoChain)  | Domain-Specific LLM-SH   |  Build lightweight, extensible, and testable LLM Agents.|
  | [TermGPT](https://github.com/Sentdex/TermGPT)   | Domain-Specific LLM-SH  | Giving LLMs like GPT-4 the ability to plan and execute terminal commands.|
  | [Botpress](https://github.com/botpress/botpress)   | Domain-Specific LLM-SH   | The open-source hub to build & deploy GPT/LLM Agents.|


#### 🧩 Language for Interaction with LLMs

LLM-LNG, on the other hand, is designed to create a language (programming or pseudo-language) for interaction with LLMs, focusing on providing users with a more concise and compact interaction channel.

* 🤖 Programming LLM-LNG
  | 🦊 Prompting Framework   | 🧚‍♂️ Subcategory | 🔍 Introduction|
  |:--------:|:-------:|:--------|
  | [LMQL](https://github.com/eth-sri/lmql)   | Programming LLM-LNG   | A language for constraint-guided and efficient LLM programming. |
  
* 🤖 Pseudocode LLM-LNG
  | 🦊 Prompting Framework   | 🧚‍♂️ Subcategory | 🔍 Introduction|
  |:--------:|:-------:|:--------|
  | [PromptLang](https://github.com/ruvnet/promptlang)   | Pseudocode LLM-LNG   | A Prompt based programming language for prompts and AI interactions. Simple and human-readable syntax for easy integration with APIs and data. |
  | [SudoLang](https://github.com/paralleldrive/sudolang-llm-support)   | Pseudocode LLM-LNG   | SudoLang is a programming language designed to collaborate with AI language models including ChatGPT, Bing Chat, Anthropic Claude, and Google Bard. It is designed to be easy to learn and use. It is also very expressive and powerful. |
  | [gpt-jargon](https://github.com/jbrukh/gpt-jargon)   | Pseudocode LLM-LNG   | Jargon is a natural language programming language specified and executed by LLMs like GPT-4. |


  
#### 🧩 Output Restrictors of LLMs

LLM-RSTR, meanwhile, achieves controlled generation by emphasizing interactions with LLMs that are of higher quality and better aligned with requirements.

* 🤖 Content LLM-RSTR
  | 🦊 Prompting Framework   | 🧚‍♂️ Subcategory | 🔍 Introduction|
  |:--------:|:-------:|:--------|
  | [NeMo-Guardrails](https://github.com/NVIDIA/NeMo-Guardrails)   | Content LLM-RSTR   | NeMo Guardrails is an open-source toolkit for easily adding programmable guardrails to LLM-based conversational systems. |
  | [Guardrails](https://github.com/guardrails-ai/guardrails)   | Content LLM-RSTR   | Guardrails is a Python package that lets a user add structure, type and quality guarantees to the outputs of large language models (LLMs).  |
  
* 🤖 Structure LLM-RSTR
  | 🦊 Prompting Framework   | 🧚‍♂️ Subcategory | 🔍 Introduction|
  |:--------:|:-------:|:--------|
  | [Guidance](https://github.com/guidance-ai/guidance)   | Structure LLM-RSTR   | guidance is a programming paradigm that offers superior control and efficiency compared to conventional prompting and chaining. It allows users to constrain generation (e.g. with regex and CFGs) as well as to interleave control (conditional, loops) and generation seamlessly.  |
  | [Promptify](https://github.com/promptslab/Promptify)   | Structure LLM-RSTR   | Prompt Engineering, Solve NLP Problems with LLM's & Easily generate different NLP Task prompts for popular generative models like GPT, PaLM, and more with Promptify. |
  | [ReLLM](https://github.com/r2d4/rellm)   | Structure LLM-RSTR   | Exact structure out of any language model completion. |
  | [TypeChat](https://github.com/microsoft/TypeChat)   | Structure LLM-RSTR   | TypeChat is a library that makes it easy to build natural language interfaces using types. |


### 🔅 Comparative Analysis of Prompting Frameworks

Comparison of state-of-the-art prompting frameworks follows three macro dimensions: 1) compatibility, 2) capabilities and features, 3) documentation and support. The more detailed dimensions are shown below. 

<div align="center">
  <img src="https://github.com/lxx0628/Prompting-Framework-Survey/blob/main/figure/dim.png" alt="dim" width="1500" />
</div>
