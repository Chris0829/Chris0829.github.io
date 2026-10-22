## Graduate Research Experience

### IGDMRec: Behavior Conditioned Item Graph Diffusion for Multimodal Recommendation
**Second student author** · IEEE Transactions on Multimedia (accepted) · Sep 2024 – Dec 2024

> **Core idea:** semantic item graphs are noisy, so treating their structure optimization as a behavior-conditioned diffusion process can denoise the graph and align it with user preferences.

<details>
<summary><b>Details</b></summary>

- Proposed the core idea and designed the overall model architecture of IGDMRec, which models structure optimization of the semantic item graph as a diffusion process.
- Extensive experiments on four datasets validated IGDMRec and its substantial improvement over baselines.

</details>

### MMCSA: Hierarchical Self-supervised Learning on Co-Semantics for Multimodal Recommendation
**First author** · IEEE Transactions on Multimedia (under review) · Jun 2025 – Nov 2025

> **Core idea:** the latent item–item structure behind multimodal interactions is under-exploited, so mining *co-semantics* — semantics jointly defined by modality and behavior — aligns multimodal features with interaction modeling.

<details>
<summary><b>Details</b></summary>

- Proposed the *co-semantics* concept to unify multimodal features and interaction behaviors.
- Developed the first co-semantic-unit subgraph mining algorithm for unsupervised discovery of consistent interaction patterns in multimodal interaction graphs.
- Designed hierarchical intra-/inter-subgraph contrastive learning fused with cross-modal alignment; corresponding Chinese invention patent submitted (first student inventor).

</details>

### CS-SHP: Collaborative Structure-Aware Semantic History Profiling for MLLM-Enhanced Recommendation
**First author** · WSDM 2027 (under review) · May 2026 – Aug 2026

> **Core idea:** frozen MLLM semantics and collaborative ranking capture complementary signals, so routing them through separate scoring paths reconciles global semantics with learned interaction structure.

<details>
<summary><b>Details</b></summary>

- Proposed the CS-SHP framework, routing global semantics, item-level history, and collaborative ranking through independent scoring pathways.
- Leveraged MLLMs to generate semantic item descriptions and user profiles.
- Propagated item representations over a semantic-behavioral relation graph into trainable history profiles, fused with a frozen LightGCN collaborative prior (64.81% average relative improvement over the strongest baselines on three Amazon datasets).

</details>

### The Structural Roots of Thermal Inequity: Linking Street Network Thermal Resilience to Socioeconomic Vulnerability
**First author** · WWW 2026 (short paper) · Oct 2025

> **Core idea:** urban thermal inequity is structurally rooted in street-network topology, so a network-science index of heat-ventilation potential can expose how infrastructure embeds environmental injustice.

<details>
<summary><b>Details</b></summary>

- Proposed the Urban Thermal Resilience Index (UTRI), a network-science metric quantifying the intrinsic heat-ventilation potential of street networks.
- Linked street-network thermal resilience to socioeconomic vulnerability in Washington, D.C., revealing significant positive spatial correlation with median household income.
- Provided quantitative evidence that heat risk is an environmental-justice issue embedded in street-network planning.

</details>

### Beyond Expected Coverage: Lower-Tail Risk Management in Fair Influence Maximization
**First author** · IEEE Transactions on Knowledge and Data Engineering (under review) · Jun 2026 – Oct 2026

> **Core idea:** fairness that only optimizes expected reach overlooks severe coverage failures under adverse diffusion, so explicit lower-tail risk measures are needed to protect disadvantaged groups.

<details>
<summary><b>Details</b></summary>

- Formalized lower-tail risk-aware influence maximization with two complementary group-level risk measures (CVaR-based lower-tail group coverage and worst-group shortage probability), scalarized into a single objective.
- Proposed the LTR-Greedy algorithm under sample-average approximation, reducing worst-group shortage by over 50% with minimal loss in total expected spread.
- Evaluated on synthetic network families and real topologies (Epinions, Slashdot, Facebook ego).

</details>

### MapPerturb: Dimension and Direction in Compact GNN Adaptation
**Sole author** · ICLR 2027 (under review) · Jul 2026 – Sep 2026

> **Core idea:** in compact GNN adaptation the number of trainable coordinates matters less than their direction, so characterizing the dimension versus alignment of weight updates reveals how to spend a tiny budget effectively.

<details>
<summary><b>Details</b></summary>

- Studied how low-dimensional update directions determine the benefit of adding trainable coordinates; parameterized weight updates around a pretrained anchor through a fixed affine map.
- Showed gradient-direction coordinates outperform random directions at matched budgets, and low-rank gradient factors match or exceed LoRA, VeRA, and full encoder tuning with 12.97–15.46× fewer stored basis values.
- Improved transductive few-shot transfer accuracy over head-only adaptation by up to 3.19 percentage points with only eight trainable encoder coordinates.

</details>

---

## Undergraduate Research Experience

### Anomaly Detection in Hydrological Monitoring Data
**CSSC Laboratory, Zhejiang University of Technology** · May 2022 – Jul 2022

<details>
<summary><b>Details</b></summary>

- Explored hydrological anomaly detection by combining hypergraph networks with reaction-diffusion equations (first research experience).

</details>

### Traffic Flow Data Imputation
**CSSC Laboratory, Zhejiang University of Technology** · Nov 2022 – Dec 2022

<details>
<summary><b>Details</b></summary>

- Studied deep-learning traffic-flow imputation with RNNs/GNNs, exploiting strong spatial correlation among nearby sensors.

</details>

### Edge-Cloud Collaborative Aquaculture Monitoring System for Fish Behavior Detection
**First student author** · IEEE SMC 2023 (CCF-C) · Jul 2022 – Oct 2022

> **Core idea:** fish behavior is a reliable indicator of health, so edge–cloud collaborative deployment of video behavior detection enables real-time monitoring in practical intensive aquaculture.

<details>
<summary><b>Details</b></summary>

- Built an IoT monitoring system with edge-cloud collaborative deployment.
- First to apply SlowFast for fish behavior detection (97.06% accuracy), deployed in intensive American shad farming in Suzhou.

</details>

### Deep Learning for Time Series Forecasting: A Survey
**First student author** · International Journal of Machine Learning and Cybernetics (2025) · Mar 2023 – Aug 2023

> **Core idea:** deep time-series forecasting is fragmented across architectures, feature extraction, and datasets, so a systematic survey can unify the field and guide newcomers.

<details>
<summary><b>Details</b></summary>

- Summarized general paradigms of deep time-series forecasting across model architectures, feature-extraction methodology, datasets, and open challenges.
- The survey has attracted **410+ citations on Google Scholar**.

</details>

### Climate-Adaptable Urban Structures and Heat Exposure
**Remote research intern** · Infrastructure, AI and Urban Nexus Lab, Clemson University · Sep 2023 – May 2024

> **Core idea:** a city's heat accumulation is shaped by the structure of its street network, so quantifying structural air-permeability links urban form to climate adaptation.

<details>
<summary><b>Details</b></summary>

- Cleaned street-network, building, and meteorological data for major North American cities; investigated urban heat islands during heatwaves.
- Proposed an air-permeability metric from urban network structure with a graph diffusion generative model — groundwork for the UTRI paper.

</details>
