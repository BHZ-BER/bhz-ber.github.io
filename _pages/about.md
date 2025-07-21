---
layout: about
title: about
permalink: /
subtitle: 
  Assistant Professor at <a href='https://www.ece.uw.edu/'>University of Washington, ECE Department</a>.<br>
  Adjunct Professor at <a href='https://www.cs.washington.edu/'>University of Washington, CSE Department</a>.<br>
  Principal Research Scientist at Nvidia.<br>

profile:
  align: right
  image: bio2.jpeg
  image_circular: true # crops the image to make it circular
  more_info: >
    

news: false # includes a list of news items
selected_papers: false # includes a list of papers marked as "selected={true}"
social: true # includes social icons at the bottom of the page
---


I'm an assistant professor at UW ECE, with adjunct appointments in CSE. I lead the Foundation Model and Reinforcement Learning Research Lab (FMRL2) at UW. 

<p style="color:red;">I am actively recruiting visiting students, PhD students, and postdoctoral researchers at the UW to work with me on LLMs, with a focus on post-training, agent, machine learning systems, or the evaluation of LLMs. If you are interested, please send me an email.</p>

I am also a principal research scientist at Nvidia. I work on star-Nemotron post-training, with a focus on reinforcement learning, agentic systems, and science of model evaluation.  
I also co-founded [Nexusflow AI](https://nexusflow.ai/) in 2023, which provides reliable AI agent solutions for enterprise use-cases.


I received my PhD from the Department of EECS, UC Berkeley. I am very fortunate to have been advised by [Prof. Jiantao Jiao](https://people.eecs.berkeley.edu/~jiantao/) and [Prof. Michael I. Jordan](http://people.eecs.berkeley.edu/~jordan/). I am a recipient of the [2023 David J. Sakrison Memorial Prize](https://www2.eecs.berkeley.edu/Students/Awards/17/) from Berkeley EECS for truly outstanding PhD research.


News: Checkout our new short course on [Post-training of LLMs](https://www.deeplearning.ai/short-courses/post-training-of-llms/), co-taught with Andrew Ng on Deeplearning.ai!


## Research Interests

I'm currently interested in the **theoretical foundations, training, serving, evaluation, and applications of foundation models**. In the past, I have also been working on **statistics**, **information theory**, and **machine learning**, with applications in game theory, robust statistics, reinforcement learning, and human-AI interactions in the past.

---

### Training

- **Starling-7B:**  
  Check out our open 7B model, [Starling-7B](https://starling.cs.berkeley.edu), which ranks first among all existing Mistral-based 7B models according to human evaluation in Chatbot Arena!  
  - Starling-7B is trained with our open-source high-quality preference dataset, [Nectar](https://huggingface.co/datasets/berkeley-nest/Nectar), using our new reward-training and policy-finetuning algorithms.

- **Athene Series:**  
  - [Athene-70B](https://huggingface.co/Nexusflow/Athene-70B): Our first chat model fine-tuned from Llama-3-70B, which [increased 30+ ELO on Chatbot Arena](https://x.com/lmarena_ai/status/1816956663821381678) and greatly improved its multi-lingual capability.  
  - [Athene-V2-72B-Chat](https://huggingface.co/Nexusflow/Athene-V2-72B-Chat): Fine-tuned from Qwen-2.5-72B. It ranks only behind Deepseek V3 & R1 (671B) among all non-reasoning open models on Chatbot Arena and is competitive with GPT-4o on benchmarks like MMLU-Pro, GPQA, AIME, IFEval, BigcodeBench, LiveBench, etc.  
  - [Athene-V2-72B-Agent](https://huggingface.co/Nexusflow/Athene-V2-72B-Agent): An agent model specializing in function calling and agentic use cases, surpassing GPT-4o in complex function-calling tasks, especially in parallel and nested calls.

---

### Evaluation

- [**Huggingface Function Calling Leaderboard**](https://huggingface.co/spaces/Nexusflow/Nexus_Function_Calling_Leaderboard): Used in the Llama-3.1 technical report for evaluating function-calling capabilities.
- [**Chatbot Arena**](https://chat.lmsys.org/): One of the most reliable platforms for evaluating models with human preferences.
- [**Arena-Hard-Auto**](https://github.com/lm-sys/arena-hard-auto): An automatic benchmark creation pipeline that uses LLM-as-a-judge to quickly evaluate model performance.
- [**Preference Proxy Evaluations**](https://arxiv.org/abs/2410.14872): A high-quality evaluation pipeline for reward models in RLHF that correlates very well with downstream RL performance.
- [**MMMG**](https://arxiv.org/abs/2505.17613): A comprehensive and reliable evaluation suite for Multitask Multimodal Generation.

---

### Theoretical Foundations

- **Fundamental Limits of RLHF:**  
  We identify the fundamental limits of RLHF and develop near-optimal algorithms with improved sample complexity for reward training [[*Z*JJ23](https://arxiv.org/abs/2301.11270)]. We also propose an alternative to Proximal Policy Optimization (PPO) for policy optimization that is more stable and sample-efficient [[*Z*SFDZJJ23](https://arxiv.org/abs/2306.02231)].

- **LLM Watermarking:**  
  We recently proposed a [statistically near-optimal algorithm for LLM watermarking](https://arxiv.org/abs/2312.07930).

---

### Serving


- **Model Routing and Caching:** 
  We analyze and propose near-optimal algorithms for caching and model multiplexing for serving large models, significantly enhancing the efficiency of inference in LLMs [[*Z*SZBJJ23](https://arxiv.org/abs/2306.02003)].
- **S-Lora:**
  We also proposed [S-Lora](https://arxiv.org/abs/2311.03285),  the algorithm and framework for serving thousands of LoRA adaptors. 

---

### Additional Research Areas

1. **Bandit and Reinforcement Learning**  
   - We study online learning and offline learning, off-policy evaluation, and inverse RL  
     \[[R*Z*MJR21](https://arxiv.org/abs/2103.12021), [M*Z*JW22](https://arxiv.org/abs/2101.07781)\].

2. **Information-theoretic Lower Bounds**  
   - We investigate achieving fundamental limits in noisy searching, sorting, and computing tasks using information-theoretic tools  
     \[[WG*Z*W22](https://arxiv.org/abs/2202.01446), [*Z*WGJW23](https://arxiv.org/abs/2306.11951)\].

3. **Statistics & Robustness**  
   - We explore techniques to enhance the resilience of AI models against malicious attacks, extending the theory in high-dimensional robust statistics [[*Z*JS22](https://arxiv.org/abs/1909.08755)].  
   - We propose efficient algorithms for outlier detection, robust mean estimation, robust covariance estimation, and robust linear regression [[*Z*JS21](https://arxiv.org/abs/2005.14073)], as well as Byzantine-robust distributed learning / distributed systems [[*Z*PWWJSJ23](https://arxiv.org/abs/2205.11765)].  
   - We design doubly-robust estimators that outperform traditional self-training pipelines in computer vision and autonomous driving [[*Z*DJWZJJ23](https://arxiv.org/abs/2306.00265)].  
   - We conduct theoretical analyses of Generative Adversarial Networks (GANs), providing insights for practical implementations [[*Z*JT19](https://arxiv.org/pdf/1901.09465)].  
   - We explore the interaction between ML systems and self-interested, strategic humans—a crucial topic in economics. By modeling and analyzing online learning in contract theory and the creator economy, I provide near-optimal regret bounds for both problems, addressing the longstanding challenge of sample complexity in online contract design  
     \[[*Z*BYWJJ23](https://arxiv.org/abs/2211.05732), [*Z*KJJ23](https://arxiv.org/abs/2305.11381)\].
