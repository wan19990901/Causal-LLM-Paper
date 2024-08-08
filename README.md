# LLM-Causality-Papers

This repository collects papers related to  **Causality (CI)** and **large language models (LLMs)**.

   
## Content
  
- [Papers](#papers)
  - [LLM](#llm)
  - [Causality](#ci)
  - [LLM and Causality](#llm-and-ci)
    - [Surveys](#surveys)
    - [LLM for Causality](#llm4ci)
    - [Causality for LLM](#ci4llm)

---

##  Papers

### LLM

- \[[arxiv](https://arxiv.org/pdf/2309.01219)\] A Survey on Hallucination in Large Language Models
`2023.09`

- \[[arxiv](https://arxiv.org/abs/2309.01029)\] Explainability for Large Language Models: A Survey. `2023.09`

### LLM and Causality

#### Surveys

- \[[arxiv](https://arxiv.org/abs/2403.09606)\] Large Language Models and Causal Inference in Collaboration: A Comprehensive Survey. `2024.03`

- \[[arxiv](https://arxiv.org/abs/2301.12351)\] Emerging Synergies in Causality and Deep Generative Models: A Survey. `2023.09`

- \[[arxiv](https://arxiv.org/abs/2305.00050)\] Causal Reasoning and Large Language Models: Opening a New Frontier for Causality. `2023.04`

- \[[arxiv](https://arxiv.org/abs/2304.05524)\] Understanding Causality with Large Language Models: Feasibility and Opportunities. `2023.04`


### LLM for Causality

#### LLM for Causal Inference

- \[[arxiv](https://arxiv.org/abs/2407.07018)\] End-To-End Causal Effect Estimation from Unstructured Natural Language Data. `2024.7`

- \[[arxiv](https://arxiv.org/abs/2310.00809)\] Towards Causal Foundation Model: on Duality between Causal Inference and Attention. `2024.6`

- \[[arxiv](https://arxiv.org/abs/2310.15117)\] Causal Inference Using LLM-Guided Discovery. `2023.10`

At the core of causal inference lies the challenge of determining reliable causal graphs solely based on observational data. Since the well-known backdoor criterion depends on the graph, any errors in the graph can propagate downstream to effect inference. In this work, we initially show that complete graph information is not necessary for causal effect inference; the topological order over graph variables (causal order) alone suffices. Further, given a node pair, causal order is easier to elicit from domain experts compared to graph edges since determining the existence of an edge can depend extensively on other variables. Interestingly, we find that the same principle holds for Large Language Models (LLMs) such as GPT-3.5-turbo and GPT-4, motivating an automated method to obtain causal order (and hence causal effect) with LLMs acting as virtual domain experts. To this end, we employ different prompting strategies and contextual cues to propose a robust technique of obtaining causal order from LLMs. Acknowledging LLMs' limitations, we also study possible techniques to integrate LLMs with established causal discovery algorithms, including constraint-based and score-based methods, to enhance their performance. Extensive experiments demonstrate that our approach significantly improves causal ordering accuracy as compared to discovery algorithms, highlighting the potential of LLMs to enhance causal inference across diverse fields.

https://ieeecai.org/2024/wp-content/pdfs/540900a460/540900a460.pdf

- \[[arxiv](https://arxiv.org/abs/2212.10534)\] DISCO: Distilling Counterfactuals with Large Language Models `2023.06`


#### LLM for Causal Discovery

- \[[arxiv](https://arxiv.org/abs/2405.01744)\] ALCM: Autonomous LLM-Augmented Causal Discovery Framework `2024.05`

https://dl.acm.org/doi/abs/10.1145/3665939.3665968

- \[[arxiv](https://arxiv.org/abs/2402.01207)\] Efficient Causal Graph Discovery Using Large Language Models `2024.02`

We propose a novel framework that leverages LLMs for full causal graph discovery. While previous LLM-based methods have used a pairwise query approach, this requires a quadratic number of queries which quickly becomes impractical for larger causal graphs. In contrast, the proposed framework uses a breadth-first search (BFS) approach which allows it to use only a linear number of queries. We also show that the proposed method can easily incorporate observational data when available, to improve performance. In addition to being more time and data-efficient, the proposed framework achieves state-of-the-art results on real-world causal graphs of varying sizes. The results demonstrate the effectiveness and efficiency of the proposed method in discovering causal relationships, showcasing its potential for broad applicability in causal graph discovery tasks across different domains.

- \[[arxiv](https://arxiv.org/abs/2402.03941)\] Discovery of the Hidden World with Large Language Models `2024.02`

Science originates with discovering new causal knowledge from a combination of known facts and observations. Traditional causal discovery approaches mainly rely on high-quality measured variables, usually given by human experts, to find causal relations. However, the causal variables are usually unavailable in a wide range of real-world applications. The rise of large language models (LLMs) that are trained to learn rich knowledge from the massive observations of the world, provides a new opportunity to assist with discovering high-level hidden variables from the raw observational data. Therefore, we introduce COAT: Causal representatiOn AssistanT. COAT incorporates LLMs as a factor proposer that extracts the potential causal factors from unstructured data. Moreover, LLMs can also be instructed to provide additional information used to collect data values (e.g., annotation criteria) and to further parse the raw unstructured data into structured data. The annotated data will be fed to a causal learning module (e.g., the FCI algorithm) that provides both rigorous explanations of the data, as well as useful feedback to further improve the extraction of causal factors by LLMs. We verify the effectiveness of COAT in uncovering the underlying causal system with two case studies of review rating analysis and neuropathic diagnosis.
  
- \[[arxiv](https://arxiv.org/abs/2402.01454)\] Integrating Large Language Models in Causal Discovery: A Statistical Causal Approach `2024.02`
  
- \[[arxiv](https://arxiv.org/abs/2307.02390)\] Causal Discovery with Language Models as Imperfect Experts `2023.06`

- \[[arxiv](https://arxiv.org/abs/2306.16902)\] From Query Tools to Causal Architects: Harnessing Large Language Models for Advanced Causal Discovery from Data
 `2023.06`

 Large Language Models (LLMs) exhibit exceptional abilities for causal analysis between concepts in numerous societally impactful domains, including medicine, science, and law. Recent research on LLM performance in various causal discovery and inference tasks has given rise to a new ladder in the classical three-stage framework of causality. In this paper, we advance the current research of LLM-driven causal discovery by proposing a novel framework that combines knowledge-based LLM causal analysis with data-driven causal structure learning. To make LLM more than a query tool and to leverage its power in discovering natural and new laws of causality, we integrate the valuable LLM expertise on existing causal mechanisms into statistical analysis of objective data to build a novel and practical baseline for causal structure learning.
We introduce a universal set of prompts designed to extract causal graphs from given variables and assess the influence of LLM prior causality on recovering causal structures from data. We demonstrate the significant enhancement of LLM expertise on the quality of recovered causal structures from data, while also identifying critical challenges and issues, along with potential approaches to address them. As a pioneering study, this paper aims to emphasize the new frontier that LLMs are opening for classical causal discovery and inference, and to encourage the widespread adoption of LLM capabilities in data-driven causal analysis.

- \[[arxiv](https://arxiv.org/abs/2303.05279)\] Can large language models build causal graphs? `2023.04`

- \[[arxiv](https://arxiv.org/abs/2301.13819)\] Causal-Discovery Performance of ChatGPT in the context of Neuropathic Pain Diagnosis `2023.02`

- \[[arxiv](https://arxiv.org/abs/2301.12473)\] Large Language Models for Biomedical Causal Graph Construction? `2023.01`

- \[[arxiv](https://arxiv.org/abs/2206.10591)\] Can Foundation Models Talk Causality? `2022.06`

- \[[arxiv](https://arxiv.org/abs/2012.05453)\] Causal BERT : Language models for causality detection between events expressed in text? `2021.01`

#### LLM for Causal Structucal Learning

- \[[arxiv](https://arxiv.org/abs/2311.11689)\] Causal Structure Learning Supervised by Large Language Model `2023.11`

- \[[arxiv](https://arxiv.org/abs/2306.07032)\] Mitigating Prior Errors in Causal Structure Learning: Towards LLM driven Prior Knowledge `2023.6`

- \[[arxiv](https://arxiv.org/abs/2102.00473)\] The impact of prior knowledge on causal structure learning `2023.3`

- \[[arxiv](https://arxiv.org/abs/2210.12530)\] LMPriors: Pre-Trained Language Models as Task-Specific Priors `2022.10`


### Causality for LLM

#### Causal Evaluation for LLM

- \[[arxiv](https://arxiv.org/abs/2401.00139)\] Is Knowledge All Large Language Models Needed for Causal Reasoning? `2024.06`

- \[[arxiv](https://arxiv.org/abs/2406.19131)\] CELLO: Causal Evaluation of Large Vision-Language Models `2024.06`

Causal reasoning is fundamental to human intelligence and crucial for effective decision-making in real-world environments. Despite recent advancements in large vision-language models (LVLMs), their ability to comprehend causality remains unclear. Previous work typically focuses on commonsense causality between events and/or actions, which is insufficient for applications like embodied agents and lacks the explicitly defined causal graphs required for formal causal reasoning. To overcome these limitations, we introduce a fine-grained and unified definition of causality involving interactions between humans and/or objects. Building on the definition, we construct a novel dataset, CELLO, consisting of 14,094 causal questions across all four levels of causality: discovery, association, intervention, and counterfactual. This dataset surpasses traditional commonsense causality by including explicit causal graphs that detail the interactions between humans and objects. Extensive experiments on CELLO reveal that current LVLMs still struggle with causal reasoning tasks, but they can benefit significantly from our proposed CELLO-CoT, a causally inspired chain-of-thought prompting strategy. Both quantitative and qualitative analyses from this study provide valuable insights for future research. Our project page is at this https URL.

- \[[arxiv](https://arxiv.org/abs/2404.06349)\] CausalBench: A Comprehensive Benchmark for Causal Learning Capability of Large Language Models? `2024.04`

Causality reveals fundamental principles behind data distributions in real-world scenarios, and the capability of large language models (LLMs) to understand causality directly impacts their efficacy across explaining outputs, adapting to new evidence, and generating counterfactuals. With the proliferation of LLMs, the evaluation of this capacity is increasingly garnering attention. However, the absence of a comprehensive benchmark has rendered existing evaluation studies being straightforward, undiversified, and homogeneous. To address these challenges, this paper proposes a comprehensive benchmark, namely CausalBench, to evaluate the causality understanding capabilities of LLMs. Originating from the causal research community, CausalBench encompasses three causal learning-related tasks, which facilitate a convenient comparison of LLMs' performance with classic causal learning algorithms. Meanwhile, causal networks of varying scales and densities are integrated in CausalBench, to explore the upper limits of LLMs' capabilities across task scenarios of varying difficulty. Notably, background knowledge and structured data are also incorporated into CausalBench to thoroughly unlock the underlying potential of LLMs for long-text comprehension and prior information utilization. Based on CausalBench, this paper evaluates nineteen leading LLMs and unveils insightful conclusions in diverse aspects. Firstly, we present the strengths and weaknesses of LLMs and quantitatively explore the upper limits of their capabilities across various scenarios. Meanwhile, we further discern the adaptability and abilities of LLMs to specific structural networks and complex chain of thought structures. Moreover, this paper quantitatively presents the differences across diverse information sources and uncovers the gap between LLMs' capabilities in causal understanding within textual contexts and numerical domains.

- \[[arxiv](https://arxiv.org/abs/2305.07375)\] Is ChatGPT a Good Causal Reasoner? A Comprehensive Evaluation. `2023.10`

- \[[arxiv](https://arxiv.org/abs/2306.05836)\] Can Large Language Models Infer Causation from Correlation? `2023.06`

- \[[arxiv](https://arxiv.org/abs/2306.05836)\] CLadder: Assessing Causal Reasoning in Language Models `2023.06`

The ability to perform causal reasoning is widely considered a core feature of intelligence. In this work, we investigate whether large language models (LLMs) can coherently reason about causality. Much of the existing work in natural language processing (NLP) focuses on evaluating commonsense causal reasoning in LLMs, thus failing to assess whether a model can perform causal inference in accordance with a set of well-defined formal rules. To address this, we propose a new NLP task, causal inference in natural language, inspired by the "causal inference engine" postulated by Judea Pearl et al. We compose a large dataset, CLadder, with 10K samples: based on a collection of causal graphs and queries (associational, interventional, and counterfactual), we obtain symbolic questions and ground-truth answers, through an oracle causal inference engine. These are then translated into natural language. We evaluate multiple LLMs on our dataset, and we introduce and evaluate a bespoke chain-of-thought prompting strategy, CausalCoT. We show that our task is highly challenging for LLMs, and we conduct an in-depth analysis to gain deeper insights into the causal reasoning abilities of LLMs. Our data is open-sourced at this https URL, and our code can be found at this https URL.

- \[[arxiv](https://arxiv.org/abs/2305.19213)\] The Magic of IF: Investigating Causal Reasoning Abilities in Large Language Models of Code `2023.05`

- \[[arxiv](https://arxiv.org/abs/2304.03439)\] Evaluating the Logical Reasoning Ability of ChatGPT and GPT-4 `2023.05`

- \[[arxiv](https://arxiv.org/abs/2308.13067)\] Causal Parrots: Large Language Models May Talk Causality But Are Not Causal `2023.05`

- \[[arxiv](https://arxiv.org/abs/2302.10198)\] Can ChatGPT Understand Too? A Comparative Study on ChatGPT and Fine-tuned BERT `2023.3`

- \[[arxiv](https://arxiv.org/abs/2206.10591)\]  Can Foundation Models Talk Causality? `2022.12`

- \[[arxiv](https://arxiv.org/abs/2112.11941)\] CRASS: A Novel Data Set and Benchmark to Test Counterfactual Reasoning of Large Language Models `2022.10`


#### Causality for Trustyworthy (better) LLM

- \[[arxiv](https://arxiv.org/abs/2307.09813)\] DAPrompt: Deterministic Assumption Prompt Learning for Event Causality Identification `2023.07`

- \[[arxiv](https://arxiv.org/abs/2305.01876)\] Causality-aware Concept Extraction based on Knowledge-guided Prompting `2023.05`

https://aclanthology.org/2023.acl-long.232/

https://ojs.aaai.org/index.php/AAAI/article/view/21389

- \[[arxiv](https://arxiv.org/abs/2310.00603)\] Faithful Explanations of Black-box NLP Models Using LLM-generated Counterfactuals `2023.10`









