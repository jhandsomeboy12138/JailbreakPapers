# Papers on Jailbreak Attacks against Large Language Models

![Awesome](https://img.shields.io/badge/Awesome-Jailbreak%20Papers-orange)
![Last Updated](https://img.shields.io/badge/Last%20Updated-April%202026-green)
![Papers](https://img.shields.io/badge/Papers-100%2B-blue)

A curated list of must-read papers on **jailbreak attacks**, **defenses**, and **evaluation** for Large Language Models (LLMs) and Multimodal Large Language Models (MLLMs). Covering research from 2022 to 2026.

> **Disclaimer**: This reading list is compiled for **academic and research purposes only**. The goal is to advance the understanding of LLM safety and promote the development of more robust AI systems.

---

## Table of Contents

- [1. Survey Papers](#1-survey-papers)
- [2. Gradient-Based / White-Box Attacks](#2-gradient-based--white-box-attacks)
- [3. Prompt-Level / Black-Box Attacks](#3-prompt-level--black-box-attacks)
  - [3.1 Template & Role-Playing Based Attacks](#31-template--role-playing-based-attacks)
  - [3.2 LLM-Assisted Iterative Attacks](#32-llm-assisted-iterative-attacks)
  - [3.3 Genetic / Evolutionary Attacks](#33-genetic--evolutionary-attacks)
  - [3.4 Encoding & Obfuscation Based Attacks](#34-encoding--obfuscation-based-attacks)
  - [3.5 Multi-Turn & In-Context Learning Attacks](#35-multi-turn--in-context-learning-attacks)
  - [3.6 Persuasion & Social Engineering Attacks](#36-persuasion--social-engineering-attacks)
  - [3.7 Fuzzing-Based Attacks](#37-fuzzing-based-attacks)
- [4. Fine-Tuning Based Attacks](#4-fine-tuning-based-attacks)
- [5. Multimodal Jailbreak Attacks](#5-multimodal-jailbreak-attacks)
- [6. Agent & System-Level Attacks](#6-agent--system-level-attacks)
- [7. Multilingual & Cross-Lingual Attacks](#7-multilingual--cross-lingual-attacks)
- [8. Defense Methods](#8-defense-methods)
  - [8.1 Input Detection & Filtering](#81-input-detection--filtering)
  - [8.2 Prompt-Level Defenses](#82-prompt-level-defenses)
  - [8.3 Decoding-Level Defenses](#83-decoding-level-defenses)
  - [8.4 Training / Alignment-Level Defenses](#84-training--alignment-level-defenses)
  - [8.5 Representation Engineering & Mechanistic Defenses](#85-representation-engineering--mechanistic-defenses)
  - [8.6 Multi-Agent & Guardrail Defenses](#86-multi-agent--guardrail-defenses)
- [9. Evaluation & Benchmarks](#9-evaluation--benchmarks)
- [10. Analysis & Understanding](#10-analysis--understanding)

---

## 1. Survey Papers

- **Jailbreak Attacks and Defenses Against Large Language Models: A Survey**
  *arXiv 2024* — *Sibo Yi, Yule Liu, Zhen Sun, Tianshuo Cong, Xinlei He, Jiaxing Song, Ke Xu, Qi Li*
  [![Paper](https://img.shields.io/badge/Paper-arXiv-red)](https://arxiv.org/abs/2407.04295)

- **Jailbreaking LLMs: A Survey of Attacks, Defenses and Evaluation (2022–2025)**
  *TechRxiv 2026* — *160+ papers systematization across security, ML, and NLP venues*
  [![Paper](https://img.shields.io/badge/Paper-TechRxiv-red)](https://www.techrxiv.org/users/1011181/articles/1373070)

- **Jailbreaking LLMs & VLMs: Mechanisms, Evaluation, and Unified Defenses** 
  *arXiv 2026* — *Three-dimensional framework covering attacks, defenses, and evaluation for both LLMs and VLMs*
  [![Paper](https://img.shields.io/badge/Paper-arXiv-red)](https://arxiv.org/abs/2601.03594)

- **Attacks, Defenses and Evaluations for LLM Conversation Safety: A Survey**
  *arXiv 2024* — *Zhichen Dong, Zhanhui Zhou, Chao Yang, Jing Shao, Yu Qiao*
  [![Paper](https://img.shields.io/badge/Paper-arXiv-red)](https://arxiv.org/abs/2402.09283)

- **A Survey of Attacks on Large Vision-Language Models: Resources, Advances, and Future Trends**
  *IEEE TNNLS 2025* — *Daizong Liu, Mingyu Yang, Xiaoye Qu, Pan Zhou, Yu Cheng, Wei Hu*
  [![Paper](https://img.shields.io/badge/Paper-arXiv-red)](https://arxiv.org/abs/2407.07403) [![Code](https://img.shields.io/badge/Code-GitHub-blue)](https://github.com/liudaizong/Awesome-LVLM-Attack)

- **A Survey on Jailbreak Attacks and Defenses against Multimodal Generative Models**
  *arXiv 2024* — *Xuannan Liu et al.*
  [![Paper](https://img.shields.io/badge/Paper-arXiv-red)](https://arxiv.org/abs/2411.09259) [![Code](https://img.shields.io/badge/Code-GitHub-blue)](https://github.com/liuxuannan/Awesome-Multimodal-Jailbreak)

- **A Survey on Agentic Security: Applications, Threats and Defenses**
  *arXiv 2025* — *Bridging applications, threats, and defenses for LLM agents*
  [![Paper](https://img.shields.io/badge/Paper-arXiv-red)](https://arxiv.org/abs/2510.06445)

---

## 2. Gradient-Based / White-Box Attacks

- **Universal and Transferable Adversarial Attacks on Aligned Language Models (GCG)**
  *ICML 2024* — *Andy Zou, Zifan Wang, Nicholas Carlini, Milad Nasr, J. Zico Kolter, Matt Fredrikson*
  [![Paper](https://img.shields.io/badge/Paper-arXiv-red)](https://arxiv.org/abs/2307.15043) [![Code](https://img.shields.io/badge/Code-GitHub-blue)](https://github.com/llm-attacks/llm-attacks)

- **AmpleGCG: Learning a Universal and Transferable Generative Model of Adversarial Suffixes for Jailbreaking Both Open and Closed LLMs**
  *NeurIPS 2024* — *Zeyi Liao, Huan Sun*
  [![Paper](https://img.shields.io/badge/Paper-arXiv-red)](https://arxiv.org/abs/2404.07921) [![Code](https://img.shields.io/badge/Code-GitHub-blue)](https://github.com/OSU-NLP-Group/AmpleGCG)

- **COLD-Attack: Jailbreaking LLMs with Stealthiness and Controllability**
  *ICML 2024* — *Xingang Guo, Fangxu Yu, Huan Zhang, Lianhui Qin, Bin Hu*
  [![Paper](https://img.shields.io/badge/Paper-arXiv-red)](https://arxiv.org/abs/2402.08679)

- **Jailbreaking Leading Safety-Aligned LLMs with Simple Adaptive Attacks**
  *ICLR 2025* — *Maksym Andriushchenko, Francesco Croce, Nicolas Flammarion*
  [![Paper](https://img.shields.io/badge/Paper-arXiv-red)](https://arxiv.org/abs/2404.02151) [![Code](https://img.shields.io/badge/Code-GitHub-blue)](https://github.com/tml-epfl/llm-adaptive-attacks)

- **Weak-to-Strong Jailbreaking on Large Language Models**
  *ICLR 2025* — *Xuandong Zhao, Xianjun Yang, Tianyu Pang, Chao Du, Lei Li, Yu-Xiang Wang, William Yang Wang*
  [![Paper](https://img.shields.io/badge/Paper-OpenReview-red)](https://openreview.net/forum?id=Nazzz5GJ4g)

- **Stronger Universal and Transferable Attacks (IRIS)**
  *NAACL 2025* — *Minimizes dot product between input embeddings and refusal activations*
  [![Paper](https://img.shields.io/badge/Paper-ACL%20Anthology-red)](https://aclanthology.org/2025.naacl-long.302.pdf)

- **Catastrophic Jailbreak of Open-Source LLMs via Exploiting Generation**
  *ICLR 2024* — *Yangsibo Huang, Samyak Gupta, Mengzhou Xia, Kai Li, Danqi Chen*
  [![Paper](https://img.shields.io/badge/Paper-arXiv-red)](https://arxiv.org/abs/2310.06987)

- **AutoDAN: Automatic and Interpretable Adversarial Attacks on Large Language Models**
  *SoReLM Workshop 2023* — *Sicheng Zhu, Ruiyi Zhang, Bang An, Gang Wu, Joe Barrow, Zichao Wang, Furong Huang, Ani Nenkova, Tong Sun*
  [![Paper](https://img.shields.io/badge/Paper-arXiv-red)](https://arxiv.org/abs/2310.15140)

- **Obscure But Effective: Jailbreaking LLMs via Obscure Characters** 
  *ICLR 2026* — *Published paper; exploits rare Unicode/classical characters to bypass safety filters*
  [![Paper](https://img.shields.io/badge/Paper-arXiv-red)](https://arxiv.org/abs/2602.22983)
  
---

## 3. Prompt-Level / Black-Box Attacks

### 3.1 Template & Role-Playing Based Attacks

- **"Do Anything Now": Characterizing and Evaluating In-The-Wild Jailbreak Prompts on Large Language Models**
  *ACM CCS 2024* — *Xinyue Shen, Zeyuan Chen, Michael Backes, Yun Shen, Yang Zhang*
  [![Paper](https://img.shields.io/badge/Paper-arXiv-red)](https://arxiv.org/abs/2308.03825)

- **DeepInception: Hypnotize Large Language Model to Be Jailbreaker**
  *NeurIPS Safe GenAI Workshop 2024* — *Xuan Li, Zhanke Zhou, Jianing Zhu, Jiangchao Yao, Tongliang Liu, Bo Han*
  [![Paper](https://img.shields.io/badge/Paper-arXiv-red)](https://arxiv.org/abs/2311.03191)

- **Not What You've Signed Up For: Compromising Real-World LLM-Integrated Applications with Indirect Prompt Injection**
  *AISec 2023* — *Kai Greshake, Sahar Abdelnabi, Shailesh Mishra, Christoph Endres, Thorsten Holz, Mario Fritz*
  [![Paper](https://img.shields.io/badge/Paper-arXiv-red)](https://arxiv.org/abs/2302.12173)

- **ArtPrompt: ASCII Art-Based Jailbreak Attacks against Aligned LLMs**
  *ACL 2024* — *Fangxu Jiang, Zhangchen Xu, Luyao Niu, Zian Lin, Bill Yuchen Lin, R. Poovendran*
  [![Paper](https://img.shields.io/badge/Paper-arXiv-red)](https://arxiv.org/abs/2402.11753)

- **ReNeLLM: Rewriting and Nesting for LLM Jailbreaking**
  *arXiv 2023* — *Peng Ding et al.*
  [![Paper](https://img.shields.io/badge/Paper-arXiv-red)](https://arxiv.org/abs/2311.08268)

- **Ignore Previous Prompt: Attack Techniques For Language Models**
  *NeurIPS ML Safety Workshop 2022* — *Fábio Perez, Ian Ribeiro*
  [![Paper](https://img.shields.io/badge/Paper-arXiv-red)](https://arxiv.org/abs/2211.09527)

### 3.2 LLM-Assisted Iterative Attacks

- **Jailbreaking Black Box Large Language Models in Twenty Queries (PAIR)**
  *ICML 2025* — *Patrick Chao, Alexander Robey, Edgar Dobriban, Hamed Hassani, George J. Pappas, Eric Wong*
  [![Paper](https://img.shields.io/badge/Paper-arXiv-red)](https://arxiv.org/abs/2310.08419)

- **Tree of Attacks: Jailbreaking Black-Box LLMs Automatically (TAP)**
  *NeurIPS 2024* — *Anay Mehrotra, Manolis Zampetakis, Paul Kassianik, Blaine Nelson, Hyrum Anderson, Yaron Singer, Amin Karbasi*
  [![Paper](https://img.shields.io/badge/Paper-arXiv-red)](https://arxiv.org/abs/2312.02119)

- **Red Teaming Language Models with Language Models**
  *EMNLP 2022* — *Ethan Perez, Saffron Huang, Francis Song, Trevor Cai, Roman Ring, John Aslanides, Amelia Glaese, Nat McAleese, Geoffrey Irving*
  [![Paper](https://img.shields.io/badge/Paper-arXiv-red)](https://arxiv.org/abs/2202.03286)

- **AutoDAN-Turbo: A Lifelong Agent for Strategy Self-Exploration to Jailbreak LLMs**
  *arXiv 2024* — *Xiaogeng Liu et al.*
  [![Paper](https://img.shields.io/badge/Paper-arXiv-red)](https://arxiv.org/abs/2410.05295) [![Code](https://img.shields.io/badge/Code-GitHub-blue)](https://github.com/SheltonLiu-N/AutoDAN)

- **RedAgent: Red Teaming Large Language Models with Context-Aware Autonomous Language Agent**
  *arXiv 2024* — *Huiyu Deng et al.*
  [![Paper](https://img.shields.io/badge/Paper-arXiv-red)](https://arxiv.org/abs/2407.16667)

- **RLbreaker: When LLM Meets DRL — Advancing Jailbreaking Efficiency via DRL-guided Search**
  *NeurIPS 2024* — *DRL-guided search outperforms genetic methods on hard queries*
  [![Paper](https://img.shields.io/badge/Paper-NeurIPS-red)](https://proceedings.neurips.cc/paper_files/paper/2024/file/2f1486343c2c942a617e4f5bb0cc64c8-Paper-Conference.pdf)

- **Mastermind: Knowledge-Driven Multi-Turn Jailbreaking on Large Language Models** 
  *arXiv 2026* — *87% avg ASR across 15 LLMs incl. GPT-5; planner-executor with knowledge accumulation*
  [![Paper](https://img.shields.io/badge/Paper-arXiv-red)](https://arxiv.org/abs/2601.05445)

### 3.3 Genetic / Evolutionary Attacks

- **AutoDAN: Generating Stealthy Jailbreak Prompts on Aligned Large Language Models**
  *ICLR 2024* — *Xiaogeng Liu, Nan Xu, Muhao Chen, Chaowei Xiao*
  [![Paper](https://img.shields.io/badge/Paper-arXiv-red)](https://arxiv.org/abs/2310.04451) [![Code](https://img.shields.io/badge/Code-GitHub-blue)](https://github.com/SheltonLiu-N/AutoDAN)

- **Open Sesame! Universal Black Box Jailbreaking of Large Language Models**
  *arXiv 2023* — *Raz Lapid, Ron Langberg, Moshe Sipper*
  [![Paper](https://img.shields.io/badge/Paper-arXiv-red)](https://arxiv.org/abs/2309.01446)

### 3.4 Encoding & Obfuscation Based Attacks

- **CipherChat: Jailbreaking LLMs via Encrypted Communication**
  *ACL 2024* — *Youliang Yuan, Wenxiang Jiao, Wenxuan Wang, Jen-tse Huang, Pinjia He, Shuming Shi, Zhaopeng Tu*
  [![Paper](https://img.shields.io/badge/Paper-arXiv-red)](https://arxiv.org/abs/2308.06463)

- **CodeChameleon: Personalized Encryption Framework for Jailbreaking LLMs**
  *arXiv 2024* — *Huijie Lv et al.*
  [![Paper](https://img.shields.io/badge/Paper-arXiv-red)](https://arxiv.org/abs/2402.16717)

- **DRA: Making Them Ask and Answer — Jailbreaking LLMs via Disguise and Reconstruction**
  *USENIX Security 2024* — *Xiaogeng Liu et al.*
  [![Paper](https://img.shields.io/badge/Paper-arXiv-red)](https://arxiv.org/abs/2402.18104)

- **FlipAttack: Jailbreak LLMs via Flipping**
  *arXiv 2024* — *Yue Liu et al.*
  [![Paper](https://img.shields.io/badge/Paper-arXiv-red)](https://arxiv.org/abs/2410.02832)

### 3.5 Multi-Turn & In-Context Learning Attacks

- **Many-Shot Jailbreaking**
  *NeurIPS 2024* — *Cem Anil, Esin Durmus, Nina Panickssery, Mrinank Sharma, et al. (Anthropic)*
  [![Paper](https://img.shields.io/badge/Paper-Anthropic-red)](https://www-cdn.anthropic.com/af5633c94ed2beb282f6a53c595eb437e8e7b630/Many_Shot_Jailbreaking__2024_04_02_0936.pdf)

- **Improved Few-Shot Jailbreaking Can Circumvent Aligned Language Models and Their Defenses (I-FSJ)**
  *NeurIPS 2024* — *Shengyun Zheng et al.*
  [![Paper](https://img.shields.io/badge/Paper-NeurIPS-red)](https://proceedings.neurips.cc/paper_files/paper/2024/file/39a3aa9dfd0280ff8fbad1d330662cac-Paper-Conference.pdf)

- **The Unlocking Spell on Base LLMs: Rethinking Alignment via In-Context Learning**
  *ICLR 2024* — *Huatao Wei, Jiaqi Han, et al.*
  [![Paper](https://img.shields.io/badge/Paper-arXiv-red)](https://arxiv.org/abs/2312.01552)

- **Paper Summary Attack: Jailbreaking LLMs through LLM Safety Papers (PSA)**
  *arXiv 2025* — *97% ASR on Claude 3.5 Sonnet, 98% on DeepSeek-R1 using academic content*
  [![Paper](https://img.shields.io/badge/Paper-arXiv-red)](https://arxiv.org/abs/2507.13474)

### 3.6 Persuasion & Social Engineering Attacks

- **How Johnny Can Persuade LLMs to Jailbreak Them: Rethinking Persuasion to Challenge AI Safety by Humanizing LLMs**
  *ACL 2024* — *Yi Zeng, Hongpeng Lin, Jingwen Zhang, Diyi Yang, Ruoxi Jia, Weiyan Shi*
  [![Paper](https://img.shields.io/badge/Paper-arXiv-red)](https://arxiv.org/abs/2401.06373)

- **Scalable and Transferable Black-Box Jailbreaks for Language Models via Persona Modulation**
  *NeurIPS SafeGenAI Workshop 2023* — *Rusheb Shah, Quentin Feuillade-Montixi, Soroush Pour, et al.*
  [![Paper](https://img.shields.io/badge/Paper-arXiv-red)](https://arxiv.org/abs/2311.03348)

- **Breaking Minds, Breaking Systems: Jailbreaking LLMs via Human-like Psychological Manipulation (HPM)**
  *arXiv 2025* — *90.8% ASR on GPT-3.5 via Big-Five personality exploitation*
  [![Paper](https://img.shields.io/badge/Paper-arXiv-red)](https://arxiv.org/abs/2512.18244)

### 3.7 Fuzzing-Based Attacks

- **GPTFuzzer: Red Teaming Large Language Models with Auto-Generated Jailbreak Prompts**
  *ISSTA 2024* — *Jiahao Yu, Xingwei Lin, Zheng Yu, Xinyu Xing*
  [![Paper](https://img.shields.io/badge/Paper-arXiv-red)](https://arxiv.org/abs/2309.10253) [![Code](https://img.shields.io/badge/Code-GitHub-blue)](https://github.com/sherdencooper/GPTFuzz)

- **PAPILLON: Efficient and Stealthy Fuzz Testing-Powered Jailbreaks for LLMs**
  *USENIX Security 2025* — *Xueluan Gong et al.*
  [![Paper](https://img.shields.io/badge/Paper-USENIX-red)](https://www.usenix.org/system/files/usenixsecurity25-gong-xueluan.pdf)

---

## 4. Fine-Tuning Based Attacks

- **Fine-Tuning Aligned Language Models Compromises Safety, Even When Users Do Not Intend To!**
  *ICLR 2024* — *Xiangyu Qi, Yi Zeng, Tinghao Xie, Pin-Yu Chen, Ruoxi Jia, Prateek Mittal, Peter Henderson*
  [![Paper](https://img.shields.io/badge/Paper-arXiv-red)](https://arxiv.org/abs/2310.03693)

- **LoRA Fine-Tuning Efficiently Undoes Safety Training in Llama 2-Chat**
  *arXiv 2023* — *Simon Lermen, Charlie Rogers-Smith, Jeffrey Ladish*
  [![Paper](https://img.shields.io/badge/Paper-arXiv-red)](https://arxiv.org/abs/2310.20624)

- **Shadow Alignment: The Ease of Subverting Safely-Aligned Language Models**
  *arXiv 2023* — *Xianjun Yang et al.*
  [![Paper](https://img.shields.io/badge/Paper-arXiv-red)](https://arxiv.org/abs/2310.02949)

- **BadLlama: Cheaply Removing Safety Fine-Tuning from Llama 2-Chat 13B**
  *arXiv 2023* — *Pranav Gade, Simon Lermen, Charlie Rogers-Smith, Jeffrey Ladish*
  [![Paper](https://img.shields.io/badge/Paper-arXiv-red)](https://arxiv.org/abs/2311.00117)

---

## 5. Multimodal Jailbreak Attacks

- **Visual Adversarial Examples Jailbreak Aligned Large Language Models**
  *AAAI 2024* — *Xiangyu Qi, Kaixuan Huang, Ashwinee Panda, Peter Henderson, Mengdi Wang, Prateek Mittal*
  [![Paper](https://img.shields.io/badge/Paper-arXiv-red)](https://arxiv.org/abs/2306.13213)

- **FigStep: Jailbreaking Large Vision-Language Models via Typographic Visual Prompts**
  *AAAI 2025* — *Yichen Gong, Delong Ran, Jinyuan Liu, Conglei Wang, Tianshuo Cong, Anyu Wang, Sisi Duan, Xiaoyun Wang*
  [![Paper](https://img.shields.io/badge/Paper-arXiv-red)](https://arxiv.org/abs/2311.05608)

- **Jailbreak in Pieces: Compositional Adversarial Attacks on Multi-Modal Language Models**
  *ICLR 2024* — *Erfan Shayegani, Yue Dong, Nael Abu-Ghazaleh*
  [![Paper](https://img.shields.io/badge/Paper-OpenReview-red)](https://openreview.net/forum?id=plmBsXHxgR)

- **Image Hijacks: Adversarial Images can Control Generative Models at Runtime**
  *ICML 2024* — *Luke Bailey, Euan Ong, Stuart Russell, Scott Emmons*
  [![Paper](https://img.shields.io/badge/Paper-arXiv-red)](https://arxiv.org/abs/2309.00236)

- **Images Are Achilles' Heel of Alignment: Exploiting Visual Vulnerabilities for Jailbreaking MLLMs**
  *ECCV 2024* — *Yifan Li, Hangyu Guo, Kun Zhou, Wayne Xin Zhao, Ji-Rong Wen*
  [![Paper](https://img.shields.io/badge/Paper-arXiv-red)](https://arxiv.org/abs/2403.09792)

- **Agent Smith: A Single Image Can Jailbreak One Million Multimodal LLM Agents Exponentially Fast**
  *ICML 2024* — *Xiangming Gu, Xiaosen Zheng, Tianyu Pang, Chao Du, Qian Liu, Ye Wang, Jing Jiang, Min Lin*
  [![Paper](https://img.shields.io/badge/Paper-arXiv-red)](https://arxiv.org/abs/2402.08567)

- **Con Instruction: Universal Jailbreaking of Multimodal Large Language Models**
  *ACL 2025* — *Adversarial samples optimized in joint embedding space*
  [![Paper](https://img.shields.io/badge/Paper-ACL%20Anthology-red)](https://aclanthology.org/2025.acl-long.146.pdf)

- **Heuristic-Induced Multimodal Risk Distribution Jailbreak Attack for MLLMs**
  *ICCV 2025* — *Teng Ma, Xiaojun Jia, Ranjie Duan, Xinfeng Li, et al.*
  [![Paper](https://img.shields.io/badge/Paper-arXiv-red)](https://arxiv.org/abs/2412.05934)

- **Distraction is All You Need for Multimodal LLM Jailbreaking (CS-DJ)**
  *CVPR 2025* — *Zuopeng Yang, Jiluan Fan, Anli Yan, Erdun Gao et al.*
  [![Paper](https://img.shields.io/badge/Paper-CVF-red)](https://openaccess.thecvf.com/content/CVPR2025/papers/Yang_Distraction_is_All_You_Need_for_Multimodal_Large_Language_Model_CVPR_2025_paper.pdf)

- **White-box Multimodal Jailbreaks Against Large Vision-Language Models**
  *ICML 2024* — *Ruofan Wang, Xingjun Ma, Hanxu Zhou, Chuanjun Ji, Guangnan Ye, Yu-Gang Jiang*
  [![Paper](https://img.shields.io/badge/Paper-OpenReview-red)](https://openreview.net/forum?id=SMOUQtEaAf)

- **MM-SafetyBench: A Benchmark for Safety Evaluation of Multimodal Large Language Models**
  *ECCV 2024* — *Xin Liu, Yichen Zhu, Jindong Gu, Yunshi Lan, Chao Yang, Yu Qiao*
  [![Paper](https://img.shields.io/badge/Paper-arXiv-red)](https://arxiv.org/abs/2311.17600)

- **SneakyPrompt: Jailbreaking Text-to-Image Generative Models**
  *IEEE S&P 2024* — *Yuchen Yang, Bo Hui, Haolin Yuan, Neil Gong, Yinzhi Cao*
  [![Paper](https://img.shields.io/badge/Paper-arXiv-red)](https://arxiv.org/abs/2305.12082)

- **Jailbreaks on Vision Language Models via Multimodal Reasoning** 
  *arXiv 2026* — *Exploits CoT prompting + ReAct-driven adaptive noising to bypass VLM safety filters*
  [![Paper](https://img.shields.io/badge/Paper-arXiv-red)](https://arxiv.org/abs/2601.22398)

---

## 6. Agent & System-Level Attacks

- **INJECAGENT: Benchmarking Indirect Prompt Injections in Tool-Integrated Large Language Model Agents**
  *ACL 2024* — *Qiusi Zhan, Zhixiang Liang, et al.*
  [![Paper](https://img.shields.io/badge/Paper-arXiv-red)](https://arxiv.org/pdf/2403.02691) [![Code](https://img.shields.io/badge/Code-GitHub-blue)](https://github.com/uiuc-kang-lab/InjecAgent)

- **Not What You've Signed Up For: Compromising Real-World LLM-Integrated Applications with Indirect Prompt Injection**
  *AISec 2023* — *Kai Greshake, Sahar Abdelnabi, Shailesh Mishra, Christoph Endres, Thorsten Holz, Mario Fritz*
  [![Paper](https://img.shields.io/badge/Paper-arXiv-red)](https://arxiv.org/abs/2302.12173)

- **iMIST: Jailbreaking LLMs through Iterative Tool-Disguised Attacks via Reinforcement Learning** 
  *arXiv 2026* — *Zhaoqi Wang, Zijian Zhang, Daqing He, Pengtao Kou, Xin Li, Jiamou Liu, Jincheng An, Yong Liu*
  [![Paper](https://img.shields.io/badge/Paper-arXiv-red)](https://arxiv.org/abs/2601.05466)

- **Bypassing Prompt Injection and Jailbreak Detection in LLM Guardrails**
  *arXiv 2025* — *Character injection and AML evasion against Azure, ProtectAI, and LLM Guard*
  [![Paper](https://img.shields.io/badge/Paper-arXiv-red)](https://arxiv.org/abs/2504.11168)

---

## 7. Multilingual & Cross-Lingual Attacks

- **Low-Resource Languages Jailbreak GPT-4**
  *arXiv 2023* — *Zheng-Xin Yong, Cristina Menghini, Stephen H. Bach*
  [![Paper](https://img.shields.io/badge/Paper-arXiv-red)](https://arxiv.org/abs/2310.02446)

- **Multilingual Jailbreak Challenges in Large Language Models**
  *ACL 2024* — *Yue Deng, Wenxuan Zhang, Sinno Jialin Pan, Lidong Bing*
  [![Paper](https://img.shields.io/badge/Paper-arXiv-red)](https://arxiv.org/abs/2310.06474)

---

## 8. Defense Methods

### 8.1 Input Detection & Filtering

- **Detecting Language Model Attacks with Perplexity**
  *arXiv 2023* — *Gabriel Alon, Michael Kamfonas*
  [![Paper](https://img.shields.io/badge/Paper-arXiv-red)](https://arxiv.org/abs/2308.14132)

- **Baseline Defenses for Adversarial Attacks Against Aligned Language Models**
  *arXiv 2023* — *Neel Jain, Avi Schwarzschild, Yuxin Wen, et al.*
  [![Paper](https://img.shields.io/badge/Paper-arXiv-red)](https://arxiv.org/abs/2309.00614)

- **Erase-and-Check: Towards Certifiable Defense Against Adversarial Prompts**
  *arXiv 2023* — *Aounon Kumar, Chirag Agarwal, Suraj Srinivas, Soheil Feizi, Himabindu Lakkaraju*
  [![Paper](https://img.shields.io/badge/Paper-arXiv-red)](https://arxiv.org/abs/2309.02705)

- **Gradient Cuff: Detecting Jailbreak Attacks on LLMs by Exploring Refusal Loss Landscapes**
  *arXiv 2024* — *Xiaomeng Hu, Pin-Yu Chen, Tsung-Yi Ho*
  [![Paper](https://img.shields.io/badge/Paper-arXiv-red)](https://arxiv.org/abs/2403.00867)

### 8.2 Prompt-Level Defenses

- **SmoothLLM: Defending Large Language Models Against Jailbreaking Attacks**
  *TMLR 2024* — *Alexander Robey, Eric Wong, Hamed Hassani, George J. Pappas*
  [![Paper](https://img.shields.io/badge/Paper-arXiv-red)](https://arxiv.org/abs/2310.03684)

- **Robust Prompt Optimization for Defending Language Models Against Jailbreaking Attacks (RPO)**
  *NeurIPS 2024* — *Andy Zhou, Bo Li, Haohan Wang*
  [![Paper](https://img.shields.io/badge/Paper-NeurIPS-red)](https://proceedings.neurips.cc/paper_files/paper/2024/file/46ed503889ab232c21c1162340ee17b2-Paper-Conference.pdf)

- **Defending ChatGPT against Jailbreak Attack via Self-Reminder**
  *arXiv 2023* — *Yueqi Xie et al.*
  [![Paper](https://img.shields.io/badge/Paper-arXiv-red)](https://arxiv.org/abs/2305.13860)

### 8.3 Decoding-Level Defenses

- **SafeDecoding: Defending against Jailbreak Attacks via Safety-Aware Decoding**
  *ACL 2024* — *Zhangchen Xu, Fengqing Jiang, Luyao Niu, Jinyuan Jia, Bill Yuchen Lin, R. Poovendran*
  [![Paper](https://img.shields.io/badge/Paper-arXiv-red)](https://arxiv.org/abs/2402.08983)

- **RAIN: Your Language Models Can Align Themselves without Finetuning**
  *ICLR 2024* — *Yuhui Li, Fangyun Wei, Jinjing Zhao, Chao Zhang, Hongyang Zhang*
  [![Paper](https://img.shields.io/badge/Paper-arXiv-red)](https://arxiv.org/abs/2309.07124)

- **SafeProbing: Defending Against Jailbreak Attacks via In-Decoding Safety-Awareness Probing** 
  *arXiv 2026* — *Surfaces latent safety signals during decoding for real-time jailbreak detection*
  [![Paper](https://img.shields.io/badge/Paper-arXiv-red)](https://arxiv.org/abs/2601.10543)

### 8.4 Training / Alignment-Level Defenses

- **Training a Helpful and Harmless Assistant with Reinforcement Learning from Human Feedback**
  *arXiv 2022* — *Yuntao Bai, Andy Jones, Kamal Ndousse, Amanda Askell, Anna Chen, et al. (Anthropic)*
  [![Paper](https://img.shields.io/badge/Paper-arXiv-red)](https://arxiv.org/abs/2204.05862)

- **Defending against Alignment-Breaking Attacks via Robustly Aligned LLM**
  *ACL 2024* — *Bochuan Cao, Yuanpu Cao, Lu Lin, Jinghui Chen*
  [![Paper](https://img.shields.io/badge/Paper-arXiv-red)](https://arxiv.org/abs/2309.14348)

- **SAID: Empowering Large Language Models with Self-Activating Internal Defense**
  *arXiv 2025* — *Training-free framework repositioning defense as model-internal activation task*
  [![Paper](https://img.shields.io/badge/Paper-arXiv-red)](https://arxiv.org/abs/2510.20129)

### 8.5 Representation Engineering & Mechanistic Defenses

- **Representation Engineering: A Top-Down Approach to AI Transparency**
  *arXiv 2023* — *Andy Zou, Long Phan, Sarah Chen, James Campbell, et al.*
  [![Paper](https://img.shields.io/badge/Paper-arXiv-red)](https://arxiv.org/abs/2310.01405)

- **Refusal in Language Models Is Mediated by a Single Direction**
  *arXiv 2024* — *Andy Arditi et al.*
  [![Paper](https://img.shields.io/badge/Paper-arXiv-red)](https://arxiv.org/abs/2406.11717)

- **Circuit Breakers: Representation Engineering for Robust Refusal**
  *arXiv 2024* — *Andy Zou et al.*
  [![Paper](https://img.shields.io/badge/Paper-arXiv-red)](https://arxiv.org/abs/2406.04313)

- **Jailbreaking Leaves a Trace: Understanding and Detecting Jailbreak Attacks from Internal Representations** 
  *arXiv 2026* — *Layer-wise analysis across GPT-J, LLaMA, Mistral, Mamba; blocks 78% of jailbreaks at inference time*
  [![Paper](https://img.shields.io/badge/Paper-arXiv-red)](https://arxiv.org/abs/2602.11495)

### 8.6 Multi-Agent & Guardrail Defenses

- **AutoDefense: Multi-Agent LLM Defense against Jailbreak Attacks**
  *arXiv 2024* — *Yifan Zeng et al.*
  [![Paper](https://img.shields.io/badge/Paper-arXiv-red)](https://arxiv.org/abs/2403.04783)

- **NeMo Guardrails: A Toolkit for Controllable and Safe LLM Applications with Programmable Rails**
  *arXiv 2023* — *Traian Rebedea, Razvan Dinu, Makesh Sreedhar, Christopher Parisien, Jonathan Cohen*
  [![Paper](https://img.shields.io/badge/Paper-arXiv-red)](https://arxiv.org/abs/2310.10501)

- **Llama Guard: LLM-based Input-Output Safeguard for Human-AI Conversations**
  *arXiv 2023* — *Hakan Inan et al. (Meta)*
  [![Paper](https://img.shields.io/badge/Paper-arXiv-red)](https://arxiv.org/abs/2312.06674)

- **Eyes Closed, Safety On: Protecting Multimodal LLMs via Image-to-Text Transformation**
  *ECCV 2024* — *Yunhao Gou et al.*
  [![Paper](https://img.shields.io/badge/Paper-arXiv-red)](https://arxiv.org/abs/2403.09572)

---

## 9. Evaluation & Benchmarks

- **HarmBench: A Standardized Evaluation Framework for Automated Red Teaming and Robust Refusal**
  *ICML 2024* — *Mantas Mazeika, Long Phan, Xuwang Yin, Andy Zou, et al.*
  [![Paper](https://img.shields.io/badge/Paper-arXiv-red)](https://arxiv.org/abs/2402.04249) [![Code](https://img.shields.io/badge/Code-GitHub-blue)](https://github.com/centerforaisafety/HarmBench)

- **JailbreakBench: An Open Robustness Benchmark for Jailbreaking Large Language Models**
  *NeurIPS 2024 (D&B Track)* — *Patrick Chao, Alexander Robey, Edgar Dobriban, Hamed Hassani, George J. Pappas, Eric Wong*
  [![Paper](https://img.shields.io/badge/Paper-arXiv-red)](https://arxiv.org/abs/2404.01318) [![Code](https://img.shields.io/badge/Code-GitHub-blue)](https://github.com/JailbreakBench/jailbreakbench)

- **JailbreakRadar: Comprehensive Assessment of Jailbreak Attacks Against LLMs**
  *ACL 2025* — *Junjie Chu, Yugeng Liu, Ziqing Yang, Xinyue Shen, Michael Backes, Yang Zhang*
  [![Paper](https://img.shields.io/badge/Paper-arXiv-red)](https://arxiv.org/abs/2402.05668)

- **A StrongREJECT for Empty Jailbreaks**
  *NeurIPS 2024* — *Alexandra Souly et al.*
  [![Paper](https://img.shields.io/badge/Paper-arXiv-red)](https://arxiv.org/abs/2402.10260)

- **EasyJailbreak: A Unified Framework for Jailbreaking Large Language Models**
  *arXiv 2024* — *Supports 11 distinct jailbreak methods*
  [![Paper](https://img.shields.io/badge/Paper-arXiv-red)](https://arxiv.org/abs/2403.12171)

- **SALAD-Bench: A Hierarchical and Comprehensive Safety Benchmark for LLMs**
  *ACL 2024* — *Tianyi Li et al.*
  [![Paper](https://img.shields.io/badge/Paper-arXiv-red)](https://arxiv.org/abs/2402.05044)

- **XSTest: A Test Suite for Identifying Exaggerated Safety Behaviours in Large Language Models**
  *NAACL 2024* — *Paul Röttger, Hannah Rose Kirk, Bertie Vidgen, Giuseppe Attanasio, Federico Bianchi, Dirk Hovy*
  [![Paper](https://img.shields.io/badge/Paper-arXiv-red)](https://arxiv.org/abs/2308.01263)

- **JailBreakV-28K: A Benchmark for Assessing the Robustness of MLLMs against Jailbreak Attacks**
  *arXiv 2024* — *Zhangchen Xu et al.*
  [![Paper](https://img.shields.io/badge/Paper-arXiv-red)](https://arxiv.org/abs/2404.03027)

- **MultiBreak: A Scalable and Diverse Multi-Turn Jailbreak Benchmark for Stress-Testing LLM Safety** 
  *ICLR 2026* — *Active learning pipeline for expanding high-quality multi-turn adversarial prompts*
  [![Paper](https://img.shields.io/badge/Paper-OpenReview-red)](https://openreview.net/pdf/49a02c4f68a8ab6fa3f6dca3f5f415dd8053a8fc.pdf)
  
---

## 10. Analysis & Understanding

- **Jailbroken: How Does LLM Safety Training Fail?**
  *NeurIPS 2023* — *Alexander Wei, Nika Haghtalab, Jacob Steinhardt*
  [![Paper](https://img.shields.io/badge/Paper-arXiv-red)](https://arxiv.org/abs/2307.02483)

- **Are Aligned Neural Networks Adversarially Aligned?**
  *NeurIPS 2023* — *Multiple authors*
  [![Paper](https://img.shields.io/badge/Paper-arXiv-red)](https://arxiv.org/abs/2306.15447)

- **How Few-shot Demonstrations Affect Prompt-based Defenses Against LLM Jailbreak Attacks** 
  *arXiv 2026* — *Systematic study of few-shot defense effectiveness across attack methods*
  [![Paper](https://img.shields.io/badge/Paper-arXiv-red)](https://arxiv.org/abs/2602.04294)

- **Learning To See But Forgetting To Follow: Visual Instruction Tuning Makes LLMs More Prone To Jailbreak Attacks**
  *arXiv 2024* — *Georgios Pantazopoulos et al.*
  [![Paper](https://img.shields.io/badge/Paper-arXiv-red)](https://arxiv.org/abs/2405.04403)

- **The Jailbreak Cookbook: A Comprehensive Encyclopedia of Jailbreak Techniques**
  *General Analysis 2025* — *Structured encyclopedia with code implementations and benchmarks*
  [![Paper](https://img.shields.io/badge/Paper-Blog-red)](https://generalanalysis.com/blog/jailbreak_cookbook)

- **Internal Safety Collapse in Frontier Large Language Models (ISC)**
  *arXiv 2026* — *Yutao Wu, Xiao Liu, Yifeng Gao, Xiang Zheng, Hanxun Huang, Yige Li, Cong Wang, Bo Li, Xingjun Ma, Yu-Gang Jiang*
  [![Paper](https://img.shields.io/badge/Paper-arXiv-red)](https://arxiv.org/abs/2603.23509) [![Code](https://img.shields.io/badge/Code-GitHub-blue)](https://wuyoscar.github.io/ISC-Bench/)

- **Do Language Models Know When They'll Refuse? Probing Introspective Awareness of Safety Boundaries**
  *arXiv 2026* — *Tanay Gondil; evaluates Claude Sonnet 4/4.5, GPT-5.2, Llama 405B with signal detection theory*
  [![Paper](https://img.shields.io/badge/Paper-arXiv-red)](https://arxiv.org/abs/2604.00228)

- **Safe in the Future, Dangerous in the Past: Dissecting Temporal and Linguistic Vulnerabilities in LLMs** ⭐ New 2026
  *arXiv 2026* — *Past-tense framing collapses safety to 15.6%; tests GPT-5.1, Gemini 3 Pro, Claude 4.5 Opus*
  [![Paper](https://img.shields.io/badge/Paper-arXiv-red)](https://arxiv.org/abs/2512.24556)

---

## Acknowledgements
**How to contribute**: Feel free to submit a pull request to add new must-read papers. Please follow the format above and ensure the paper is of high quality (published in top venues or highly cited on arXiv).
