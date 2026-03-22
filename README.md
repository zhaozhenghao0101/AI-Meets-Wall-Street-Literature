# When AI Meets Wall Street: A Survey on Trustworthy AI in Fintech

[![Paper](https://img.shields.io/badge/Paper-PDF-red.svg)](https://arxiv.org/abs/xxxx.xxxxx) This repository is the official curated paper list for the survey **"When AI Meets Wall Street: A Survey on Trustworthy AI in Fintech."** Modern financial AI systems operate as continuously deployed, automation-amplified pipelines. Based on our research, this repository systematically maps security and robustness threats across the end-to-end financial AI lifecycle. We categorize adversarial vulnerabilities into three operational phases: the model training phase, the model deployment and inference phase, and the model monitoring and maintenance phase.

## 📝 Citation

If you find this repository or our survey helpful for your research, please consider citing our paper:

```bibtex
@article{anonymous2026when,
  title={When AI Meets Wall Street: A Survey on Trustworthy AI in Fintech},
  author={Anonymous Author(s)}, 
  journal={ACM Computing Surveys},
  year={2026}
}
```

## 📑 Table of Contents

- [Phase 1: Model Training Phase](#phase-1-model-training-phase)
  - [Data Poisoning Attack](#data-poisoning-attack)
  - [Model Poisoning Attack](#model-poisoning-attack)
- [Phase 2: Model Deployment and Inference Phase](#phase-2-model-deployment-and-inference-phase)
  - [Adversarial Attacks on Decision Boundary](#adversarial-attacks-on-decision-boundary)
- [Phase 3: Operation and Monitoring Phase](#phase-3-operation-and-monitoring-phase)
  - [Prompt Injection (LLM Workflow)](#prompt-injection-llm-workflow)
  - [Deepfake Verification Layer (KYC)](#deepfake-verification-layer-kyc)

---

## 📚 Taxonomy & Paper List

### Phase 1: Model Training Phase 
In this stage, algorithms ingest historical financial data to construct the core decision-making logic. [cite: 492] The primary threats emerge from manipulating the underlying historical records or hijacking the decentralized optimization process. 

#### Data Poisoning Attack [cite: 336]
Contaminating historical datasets (altering input features or target labels) to embed malicious statistical associations into the model's logic. [cite: 505, 506]
* **S1: Label-Level Data Poisoning** [cite: 335]
  * *Investigating machine learning attacks on financial time series models* by Gallagher et al. [cite: 581, 2361]
  * *Detecting and preventing data poisoning attacks on AI models* by Kure et al. [cite: 586, 2377]
* **S2: Feature-Level Data Poisoning** [cite: 337]
  * *Data poisoning attacks against autoregressive models* by Alfeld et al. [cite: 598, 1565]
  * *Sonic: Fast and transferable data poisoning on clustering algorithms* by Villani et al. [cite: 661, 662, 2492]
* **S3: Instance-Level Data Poisoning** [cite: 338]
  * *Get a model! model hijacking attack against machine learning models* by Salem et al. [cite: 676, 2458]
  * *Impact of backdoor attacks on face classification models through training data poisoning* by Kutbi [cite: 681, 2387]
  * *Effectiveness Evaluation of Black-Box Data Poisoning Attack on Machine Learning Models* by Zhan et al. [cite: 686, 2546]
  * *Latent diffusion model-based data poisoning attack against QoS-aware cloud API recommender system* by Chen et al. [cite: 744, 1604]

#### Model Poisoning Attack [cite: 339]
Directly compromising the mathematical optimization trajectory in distributed architectures (e.g., Federated Learning) to inject malicious logic or backdoors. [cite: 826, 838]
* **S4: Global Gradient Model Poisoning** [cite: 340]
  * *Model poisoning attacks to federated learning via multi-round consistency* by Xie et al. [cite: 895, 2517]
  * *Enhanced model poisoning attack and multi-strategy defense in federated learning* by Yang et al. [cite: 900, 2530]
* **S5: Fragment / Coordinate-Level Model Poisoning** [cite: 341]
  * *FMPA: Fragment Model Poisoning Attack in Federated Learning* by Ren et al. [cite: 946, 2452]
  * *Sine: Similarity is not enough for mitigating local model poisoning attacks in federated learning* by Kasyap and Tripathy [cite: 950, 2345]
* **S6: Backdoor Trigger-Based Model Poisoning** [cite: 342]
  * *Universal adversarial backdoor attacks to fool vertical federated learning* by Chen et al. [cite: 988, 1600]
  * *Stealthy Backdoors in Vertical Federated Learning* by Yang et al. [cite: 993, 2534]
  * *Improved Distributed Backdoor Attacks in Federated Learning by Density-Adaptive Data Poisoning and Projection-Based Gradient Updating* by Wang et al. [cite: 998, 2501]
---

### Phase 2: Model Deployment and Inference Phase
Financial AI models operate on highly dynamic time series and structured transaction data in this phase. Attackers craft localized perturbations under domain constraints to induce misclassification or erroneous predictions. 

#### Adversarial Attacks on Decision Boundary
* **S7: Input Manipulation Attacks**
  * *Adversarial attacks on deep models for financial transaction records* by Fursov et al. [cite: 1625]
  * *Improving the robustness of financial models through identification of the minimal vulnerable feature set* by Pandey et al. [cite: 1726]
  * *Adversarial Machine Learning Attacks on Financial Reporting via Maximum Violated Multi-Objective Attack* by Raff et al. [cite: 1750]
* **S8: Single-Step Adversarial Attack**
  * *Explaining and harnessing adversarial examples* by Goodfellow et al. [cite: 1639]
  * *Investigating machine learning attacks on financial time series models* by Gallagher et al. [cite: 1628]
* **S9: Optimisation-Based Adversarial Attack**
  * *Intriguing properties of neural networks* by Szegedy et al. [cite: 2469]
  * *Towards deep learning models resistant to adversarial attacks* by Madry et al. [cite: 2436]
  * *Adversarial attacks on machine learning systems for high-frequency trading* by Goldblum et al. [cite: 1637]
  * *FRAUD-RLA: A new reinforcement learning adversarial attack against credit card fraud detection* by Lunghi et al. [cite: 2434]
* **S10: Transfer-Based Adversarial Attack**
  * *Adversarial Attacks on Deep Algorithmic Trading Policies* by Piazza et al. [cite: 1747]
  * *Foe for Fraud: Transferable Adversarial Attacks in Credit Card Fraud Detection* by Fok et al. [cite: 1623]

---

### Phase 3: Operation and Monitoring Phase
This phase represents the operational steady-state where AI systems actively interact with users and execute automated workflows. Vulnerabilities arise from the system's reliance on the semantic integrity of its inputs.

#### Prompt Injection (LLM Workflow)
Exploiting the control-data confusion in LLM-mediated workflows to override the system's original operating instructions. [cite: 1664]
* **S11: Character / Symbol-Level**
  * *Evaluating prompt injection safety in large language models using the promptbench dataset* by Sang et al. [cite: 1673, 2575, 2576]
  * *Bypassing LLM guardrails: An empirical analysis of evasion attacks against prompt injection and jailbreak detection systems* by Hackett et al. [cite: 1678, 2460, 2461]
* **S12: Word / Phrase-Level**
  * *Semantics-Preserving Adversarial Attacks on Event-Driven Stock Prediction Models* by Liu et al. [cite: 1690, 2412, 2413]
  * *Adversarial News and Lost Profits: Manipulating Headlines in LLM-Driven Algorithmic Trading* by Rizvani et al. [cite: 1720, 2553, 2554]
  * *Optimization-based prompt injection attack to llm-as-a-judge* by Shi et al. [cite: 1725, 2577, 2579]
* **S13: Sentence / Instruction Level**
  * *Prompt packer: Deceiving llms through compositional instruction with hidden attacks* by Jiang et al. [cite: 1761, 2386, 2387]
  * *'Do as I say not as I do': A Semi-Automated Approach for Jailbreak Prompt Attack against Multimodal LLMs* by Chiu et al. [cite: 1767, 2355, 2356]
  * *Pleak: Prompt leaking attacks against large language model applications* by Hui et al. [cite: 1770, 2374, 2375]
* **S14: Context Chain Injection**
  * *Simple prompt injection attacks can leak personal data observed by llm agents during task execution* by Alizadeh et al. [cite: 1779, 2314, 2315]
  * *Adaptive attacks break defences against indirect prompt injection attacks on llm agents* by Zhan et al. [cite: 1838, 2549, 2552]
  * *Autohijacker: Automatic indirect prompt injection against black-box llm agents* by Liu et al. [cite: 1845, 2419, 2420]

#### Deepfake Verification Layer (KYC)
Utilizing deep generative models to synthesize or manipulate hyper-realistic multimedia content, compromising the integrity of remote identity verification systems. [cite: 1863, 1866]
* **S15: Latent Identity-Level Synthesis**
  * *Arc2face: A foundation model for id-consistent human faces* by Papantoniou et al. [cite: 1927, 2445, 2447]
  * *Master face attacks on face recognition systems* by Nguyen et al. [cite: 1992, 2465, 2466]
  * *Diffmorpher: Unleashing the capability of diffusion models for image morphing* by Zhang et al. [cite: 1995, 2554, 2557]
* **S16: Feature / Attribute-Level Transfer**
  * *Diffswap: High-fidelity and controllable face swapping via 3d-aware masked diffusion* by Zhao et al. [cite: 2005, 2564, 2567]
  * *Seeing is living? rethinking the security of facial liveness verification in the deepfake era* by Li et al. [cite: 2009, 2396, 2397]
* **S17: Adversarial Anti-Forensic Generation**
  * *Physical-world optical adversarial attacks on 3d face recognition* by Li et al. [cite: 2074, 2404, 2405]
  * *Efficient decision-based black-box adversarial attacks on face recognition* by Dong et al. [cite: 2078, 2316, 2317]

---

## 🤝 Contributing & Contact
We welcome pull requests to keep this repository updated with the latest research in the field! If you have any questions, please feel free to open an issue or contact the authors.
