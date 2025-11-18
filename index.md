---
layout: page
permalink: / 
---

<div style="float: right; margin-left: 20px; margin-bottom: 20px;">
    <img src="/assets/img/photo.jpg" alt="Runyu Lu Photo" width="180"/> 
</div>

Hello! I'm **Runyu Lu (陆润宇)**, a Ph.D. Candidate specializing in **Game Theory and Reinforcement Learning** at the University of Chinese Academy of Sciences (UCAS), supervised by **Prof. Dongbin Zhao**.

My research focuses on **equilibrium learning**, aiming to develop model-based or offline learning algorithms with **last-iterate convergence guarantees** in dynamic games, which facilitate deep RL implementations. I also proposed the **Equilibrium Policy Generalization** paradigm for real-time robust strategies.

Prior to my Ph.D., I earned my B.Eng. in Computer Science and Technology from the University of Chinese Academy of Sciences.

---

## News

* **2025**
    * **Oct 15, 2025:** Our paper **"R2PS: Worst-Case Robust Real-Time Pursuit Strategies under Partial Observability"** submitted to **ICLR 2026** (under review).
    * **Sept 01, 2025:** Our paper **"Equilibrium Policy Generalization:..."** was accepted to **NeurIPS 2025**.
    * **Jun 25, 2025:** Our paper **"Constrained Exploitability Descent:..."** was accepted to **ICML 2025**.
    * **Apr 01, 2025:** Our paper **"Divergence-Regularized Discounted Aggregation:..."** was accepted to **ICLR 2025**.

* **2024**
    * **Dec 20, 2024:** Our journal paper **"Last-Iterate Convergence..."** was accepted by **IEEE TNNLS**.
    * **Sept 20, 2024:** Started development on the **Hierarchical Campus Security System** project.

---

## Selected Publications

### Conference Paper

* **[NeurIPS 2025] Equilibrium Policy Generalization: A Reinforcement Learning Framework for Cross-Graph Zero-Shot Generalization in Pursuit-Evasion Games.**
    * **Lu, R.**, Zhang, P., Shi, R., et al. (First Author)
    * *The 39th Annual Conference on Neural Information Processing Systems (NeurIPS)*, 2025.
    * [Paper Link] [Code] [Project Page]
    
    > **Abstract:** Equilibrium learning in adversarial games is an important topic widely examined in the fields of game theory and reinforcement learning (RL). Pursuit-evasion game (PEG), as an important class of real-world games from the fields of robotics and security, requires exponential time to be accurately solved. When the underlying graph structure varies, even the state-of-the-art RL methods require recomputation or at least fine-tuning, which can be time-consuming and impair real-time applicability. This paper proposes an Equilibrium Policy Generalization (EPG) framework to effectively learn a generalized policy with robust cross-graph zero-shot performance. In the context of PEGs, our framework is generally applicable to both pursuer and evader sides in both no-exit and multi-exit scenarios. These two generalizability properties, to our knowledge, are the first to appear in this domain. The core idea of the EPG framework is to train an RL policy across different graph structures against the equilibrium policy for each single graph. To construct an equilibrium oracle for single-graph policies, we present a dynamic programming (DP) algorithm that provably generates pure-strategy Nash equilibrium with near-optimal time complexity. To guarantee scalability with respect to pursuer number, we further extend DP and RL by designing a grouping mechanism and a sequence model for joint policy decomposition, respectively. Experimental results show that, using equilibrium guidance and a distance feature proposed for cross-graph PEG training, the EPG framework guarantees desirable zero-shot performance in various unseen real-world graphs. Besides, when trained under an equilibrium heuristic proposed for the graphs with exits, our generalized pursuer policy can even match the performance of the fine-tuned policies from the state-of-the-art PEG methods.

* **[ICML 2025] Constrained Exploitability Descent: An Offline Reinforcement Learning Method for Finding Mixed-Strategy Nash Equilibrium.**
    * **Lu, R.**, Zhu Y., Zhao D. (First Author)
    * *The 42nd International Conference on Machine Learning (ICML)*, 2025.
    * [Paper Link] [Code]

    > **Abstract:** This paper proposes Constrained Exploitability Descent (CED), a model-free offline reinforcement learning (RL) algorithm for solving adversarial Markov games (MGs). CED combines the game-theoretical approach of Exploitability Descent (ED) with policy constraint methods from offline RL. While policy constraints can perturb the optimal pure-strategy solutions in single-agent scenarios, we find the side effect less detrimental in adversarial games, where the optimal policy can be a mixed-strategy Nash equilibrium. We theoretically prove that, under the uniform coverage assumption on the dataset, CED converges to a stationary point in deterministic two-player zero-sum Markov games. We further prove that the min-player policy at the stationary point follows the property of mixed-strategy Nash equilibrium in MGs. Compared to the model-based ED method that optimizes the max-player policy, our CED method no longer relies on a generalized gradient. Experiments in matrix games, a tree-form game, and an infinite-horizon soccer game verify that CED can find an equilibrium policy for the min-player as long as the offline dataset guarantees uniform coverage. Besides, CED achieves a significantly lower NashConv compared to an existing pessimism-based method and can gradually improve the behavior policy even under non-uniform data coverages. When combined with neural networks, CED also outperforms behavior cloning and offline self-play in a large-scale two-team robotic combat game.

* **[ICLR 2025] Divergence-Regularized Discounted Aggregation: Equilibrium Finding in Multiplayer Partially Observable Stochastic Games.**
    * **Lu, R.**, Zhu Y., Zhao D. (First Author)
    * *The 13th International Conference on Learning Representations (ICLR)*, 2025.
    * [Paper Link] [Code]
    
    > **Abstract:** This paper presents Divergence-Regularized Discounted Aggregation (DRDA), a multi-round learning system for solving partially observable stochastic games (POSGs). DRDA is based on action values and applicable to multiplayer POSGs, which can unify normal-form games (NFGs), extensive-form games (EFGs) with perfect recall, and Markov games (MGs). In each single round, DRDA can be viewed as a discounted variant of Follow the Regularized Leader (FTRL) under a general value function for POSGs. While previous studies on discounted FTRL have demonstrated its last-iterate convergence towards quantal response equilibrium (QRE) in NFGs, this paper extends the theoretical results to POSGs under divergence regularization and generalizes the QRE concept of Nash distribution. The linear last-iterate convergence of single-round DRDA to its rest point is proved under the assumption on the hypomonotonicity of the game. When the rest point is unique, it induces the unique Nash distribution defined in the POSG, which has a bounded deviation from Nash equilibrium (NE). Under multiple learning rounds, DRDA keeps replacing the base policy for divergence regularization with the policy at the rest point in the previous round. It is further proved that the limit point of multi-round DRDA must be an exact NE (rather than a QRE). In experiments, discrete-time DRDA can converge to NE at a near-exponential rate in (multiplayer) NFGs and outperform the existing baselines for EFGs, MGs, and typical POSGs.

* **[Under Review] R2PS: Worst-Case Robust Real-Time Pursuit Strategies under Partial Observability.**
    * **Lu, R.**, Shi, R., Zhu Y., Zhao D. (submitted to ICLR 2026)
    * [Paper Link] [Code]
    
    > **Abstract:** Computing worst-case robust strategies in pursuit-evasion games (PEGs) is time-consuming, especially when real-world factors like partial observability are considered. While important for general security purposes, real-time applicable pursuit strategies for graph-based PEGs are currently missing when the pursuers only have imperfect information about the evader's position. Although state-of-the-art reinforcement learning (RL) methods like Equilibrium Policy Generalization (EPG) and Grasper provide guidelines for learning graph neural network (GNN) policies robust to different game dynamics, they are restricted to the scenario of perfect information and do not take into account the possible case where the evader can predict the pursuers' actions. This paper introduces the first approach to worst-case robust real-time pursuit strategies (R2PS) under partial observability. We first prove that a traditional dynamic programming (DP) algorithm for solving Markov PEGs maintains optimality under the asynchronous moves by the evader. Then, we extend the DP pursuit strategies to a partially observable setting through preserving beliefs about the evader's possible positions. Finally, we embed the belief preservation mechanism into the state-of-the-art EPG framework to finish our R2PS learning scheme, which leads to a real-time pursuer policy through cross-graph reinforcement learning against the asynchronous-move DP evasion strategies. Experiments under different training sets reveal that using the extended DP pursuers as guidance improves the training efficiency under partial observability. After reinforcement learning, our policy achieves robust zero-shot generalization to unseen real-world graph structures and consistently outperforms the policy directly trained on the test graphs by the existing game RL approach, even against a best-responding evader.

### Journal Paper

* **[IEEE TNNLS 2025] Last-Iterate Convergence to Approximate Nash Equilibria in Multiplayer Imperfect Information Games.**
    * **Lu, R.**, Zhu, Y., Zhao D, et al.
    * *IEEE Transactions on Neural Networks and Learning Systems (TNNLS)*, Vol. 36, No. 8, 2025.
    * [Journal Link]
    
    > **Abstract:** Imperfect information and multiple players are the two common features of real-world games. However, few of the existing game-theoretic methods are applicable to multiplayer imperfect information games (IIGs) when it comes to finding Nash equilibria. Moreover, the commonly used methods that rely on average-iterate convergence are not conducive to deep reinforcement learning (DRL), which is widely applied to large-scale problems, as it is costly to preserve average policies under function approximation. To deal with these problems, we construct a continuous-time dynamic named \textit{imperfect-information exponential-decay score-based learning} (IESL) by considering the concept of Nash distribution (a type of quantal response equilibrium) in IIGs. Theoretically, we prove the last-iterate convergence of IESL to approximate Nash equilibria in multiplayer IIGs under the assumption of individual concavity. Empirically, we verify that IESL converges in six poker scenarios, with the ultimate NashConv lower than that of the comparative methods (including counterfactual regret minimization (CFR), replicator dynamics (RD), and their variants) in multiplayer Leduc hold'em. When compared to the existing equilibrium-finding algorithms in multiplayer normal-form games, IESL also demonstrates a more stable performance. Besides, we observe a trade-off between the difficulty of IESL's last-iterate convergence and the NashConv of the convergent policies, which aligns with our convergence analysis based on the hypomonotonicity of the game.

---
