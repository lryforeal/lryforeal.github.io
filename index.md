---
layout: page
permalink: / 
---

<div style="float: right; margin-left: 20px; margin-bottom: 20px;">
    <img src="/assets/img/photo.jpg" alt="Runyu Lu Photo" width="180"/> 
</div>

Hello! I'm **Runyu Lu (陆润宇)**, a Ph.D. Candidate specializing in **Game Theory and Reinforcement Learning** at the University of Chinese Academy of Sciences (UCAS), supervised by **Prof. Dongbin Zhao**.

My research focuses on **equilibrium learning**, aiming to develop model-based, offline, or online learning algorithms with **last-iterate convergence guarantees** in dynamic games, which facilitate deep RL implementations. I also proposed the **Equilibrium Policy Generalization** paradigm for real-time robust strategies.

Prior to my Ph.D., I earned my B.Eng. in Computer Science and Technology from the University of Chinese Academy of Sciences.

---

## 📰 News

* **[Jan 2026]** Our paper "**R2PS: Worst-Case Robust Real-Time Pursuit Strategies under Partial Observability**" was accepted to **ICLR 2026**!
* 
* **[Nov 2025]** I attended the **7th International Conference in Distributed Artificial Intelligence (DAI 2025)** at King's College London, UK!
    * Organized the workshop "**LLMs in Games: Reasoning, Strategy, and Distributed Intelligence**" (Nov 21)
    * Gave a talk on "**Divergence-Regularized Reinforcement Learning for Equilibrium Policies in Adversarial Games**" for the workshop.
    * Made an oral presentation for our accepted paper, "**ARAC: Adaptive Regularized Multi-Agent Soft Actor-Critic in Graph-Structured Adversarial Games**" (Nov 24).

* **[Sep 2025]** Our paper "**Equilibrium Policy Generalization: A Reinforcement Learning Framework for Cross-Graph Zero-Shot Generalization in Pursuit-Evasion Games**" was accepted to **NeurIPS 2025**!

---

## 📚 Selected Publications

### Conference Papers

* **[NeurIPS 2025] Equilibrium Policy Generalization: A Reinforcement Learning Framework for Cross-Graph Zero-Shot Generalization in Pursuit-Evasion Games.**
    * **Lu, R.**, Zhang, P., Shi, R., et al.
    * *The 39th Annual Conference on Neural Information Processing Systems (NeurIPS)*, 2025.
    * [openreview.net/pdf?id=z67on2D0j1](https://openreview.net/pdf?id=z67on2D0j1)

    **Summary:** Proposes the **Equilibrium Policy Generalization (EPG)** framework, aiming to find robust policy representation across changing game dynamics. Under pursuit-evasion games (PEGs), EPG enables **cross-graph zero-shot generalization** of policies by training against the opponents generated from a near-optimal equilibrium oracle. Establishing the first two generalizability properties in this domain. Designing a grouping mechanism and a sequence model for scalability.

* **[ICML 2025] Constrained Exploitability Descent: An Offline Reinforcement Learning Method for Finding Mixed-Strategy Nash Equilibrium.**
    * **Lu, R.**, Zhu Y., Zhao D.
    * *The 42nd International Conference on Machine Learning (ICML)*, 2025.
    * [openreview.net/pdf?id=unUW6MC7Su](https://openreview.net/pdf?id=unUW6MC7Su)

    **Summary:** Introduces **Constrained Exploitability Descent (CED)**, a model-free **offline RL** algorithm for adversarial Markov games (MGs). Theoretically proves that CED converges to a stationary point where the min-player policy exhibits the **mixed-strategy Nash equilibrium** property. CED significantly outperforms existing pessimism-based and self-play methods in offline equilibrium finding.

* **[ICLR 2025] Divergence-Regularized Discounted Aggregation: Equilibrium Finding in Multiplayer Partially Observable Stochastic Games.**
    * **Lu, R.**, Zhu Y., Zhao D.
    * *The 13th International Conference on Learning Representations (ICLR)*, 2025.
    * [openreview.net/pdf?id=KD5nJUgeW4](https://openreview.net/pdf?id=KD5nJUgeW4)

    **Summary:** Presents **Divergence-Regularized Discounted Aggregation (DRDA)**, a multi-round learning system for **Multiplayer Partially Observable Stochastic Games (POSGs)**. Extends discounted FTRL theory to POSGs, proving last-iterate convergence to Nash distribution in a single round, and convergence to an **exact Nash Equilibrium (NE)** over multiple rounds.

### Journal Paper

* **[IEEE TNNLS 2024] Last-Iterate Convergence to Approximate Nash Equilibria in Multiplayer Imperfect Information Games.**
    * **Lu, R.**, Zhu, Y., Zhao D, et al.
    * *IEEE Transactions on Neural Networks and Learning Systems (TNNLS)*, Vol. 36, No. 8, 2025.
    * [ieeexplore.ieee.org/abstract/document/10806634](https://ieeexplore.ieee.org/abstract/document/10806634)
    
    **Summary:** Constructs the continuous-time dynamic **Imperfect-information Exponential-decay Score-based Learning (IESL)** for **multiplayer imperfect information games (IIGs)**. Proves **last-iterate convergence** to approximate Nash equilibria, which is highly beneficial for deep RL implementations. Empirically verified to outperform CFR and RD variants in multiplayer poker.

### Working Paper

* **[ICLR 2026] R2PS: Worst-Case Robust Real-Time Pursuit Strategies under Partial Observability.**
    * **Lu, R.**, Shi, R., Zhu Y., Zhao D. (accepted to ICLR 2026)
    * [arxiv.org/pdf/2511.17367](https://arxiv.org/pdf/2511.17367)

    **Summary:** Proposes **Worst-Case Robust Real-Time Pursuit Strategies (R2PS)** for graph-based PEGs under **partial observability** and **asynchronous moves**. Integrates a belief preservation mechanism with the EPG framework to learn robust, real-time GNN policies against asynchronous-move evasion strategies, achieving superior zero-shot generalization.
