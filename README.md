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
In this stage, algorithms ingest historical financial data to construct the core decision-making logic. The primary threats emerge from manipulating the underlying historical records or hijacking the decentralized optimization process.

#### Data Poisoning Attack
Contaminating historical datasets (altering input features or target labels) to embed malicious statistical associations into the model's logic.
* **S1: Label-Level Data Poisoning**
  * *(Papers will be added here)*
* **S2: Feature-Level Data Poisoning**
  * *(Papers will be added here)*
* **S3: Instance-Level Data Poisoning**
  * *(Papers will be added here)*

#### Model Poisoning Attack
Directly compromising the mathematical optimization trajectory in distributed architectures (e.g., Federated Learning) to inject malicious logic or backdoors.
* **S4: Global Gradient Model Poisoning**
  * *(Papers will be added here)*
* **S5: Fragment / Coordinate-Level Model Poisoning**
  * *(Papers will be added here)*
* **S6: Backdoor Trigger-Based Model Poisoning**
  * *(Papers will be added here)*

---

### Phase 2: Model Deployment and Inference Phase
Financial AI models operate on highly dynamic time series and structured transaction data in this phase. Attackers craft localized perturbations under domain constraints to induce misclassification or erroneous predictions.

#### Adversarial Attacks on Decision Boundary
* **S7: Input Manipulation Attacks**
  * *(Papers will be added here)*
* **S8: Single-Step Adversarial Attack**
  * *(Papers will be added here)*
* **S9: Optimisation-Based Adversarial Attack**
  * *(Papers will be added here)*
* **S10: Transfer-Based Adversarial Attack**
  * *(Papers will be added here)*

---

### Phase 3: Operation and Monitoring Phase
This phase represents the operational steady-state where AI systems actively interact with users and execute automated workflows. Vulnerabilities arise from the system's reliance on the semantic integrity of its inputs.

#### Prompt Injection (LLM Workflow)
Exploiting the control-data confusion in LLM-mediated workflows to override the system's original operating instructions.
* **S11: Character / Symbol-Level**
  * *(Papers will be added here)*
* **S12: Word / Phrase-Level**
  * *(Papers will be added here)*
* **S13: Sentence / Instruction Level**
  * *(Papers will be added here)*
* **S14: Chain / Indirect Injection**
  * *(Papers will be added here)*

#### Deepfake Verification Layer (KYC)
Utilizing deep generative models to synthesize or manipulate hyper-realistic multimedia content, compromising the integrity of remote identity verification systems.
* **S15: Latent Identity-Level Synthesis**
  * *(Papers will be added here)*
* **S16: Feature / Attribute-Level Transfer**
  * *(Papers will be added here)*
* **S17: Adversarial Anti-Forensic Generation**
  * *(Papers will be added here)*

---

## 🤝 Contributing & Contact
We welcome pull requests to keep this repository updated with the latest research in the field! If you have any questions, please feel free to open an issue or contact the authors.
