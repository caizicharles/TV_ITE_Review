# A Review of Deep Learning for Individualized Treatment Effect Estimation in Healthcare Time Series

![Submitted to ACM Computing Surveys](https://img.shields.io/badge/Submitted_to-ACM_Computing_Surveys-blue)
![Last Updated](https://img.shields.io/badge/Last_Updated-April_2026-brightgreen)
![Papers](https://img.shields.io/badge/Papers-35-red)

**Authors:** Zi Cai, Yu Liu, and Tingting Zhu

**Affiliation:** [Laboratory of AI for Digital Healthcare](https://eng.ox.ac.uk/ai4dh), Institute of Biomedical Engineering, Department of Engineering Science, University of Oxford

---

## Abstract

The proliferation of healthcare time series data presents a transformative opportunity for personalized healthcare. However, utilizing these observational data for clinical decision support requires moving beyond risk prediction to causal inference. In particular, estimating time-varying individual treatment effects is crucial for answering "what-if" questions in dynamic settings, where patient states and treatment efficacy evolve continuously over time. Traditional statistical and machine learning methods face well-documented difficulties in capturing the long-range temporal dependencies, high dimensionality, and non-linear treatment-response dynamics characteristic of such data. Deep learning has emerged as a powerful paradigm for addressing these challenges, motivating a rapidly growing body of work on time-varying causal inference from healthcare time series data. This review aims to provide a systematic overview of deep learning for time-varying ITE estimation in healthcare, connecting theoretical foundations with methodological practice. We first establish the theoretical foundations, then present a taxonomy of deep learning methodologies, followed by an analysis of current clinical applications and model evaluation practices. Finally, we discuss key unresolved challenges and outline a roadmap for future research on time-varying ITE estimation.

---

## Citation

If you find this review useful, please use the following to cite our work:

```bibtex
@article{cai2026review,
  title     = {A Review of Deep Learning for Individualized Treatment Effect Estimation in Healthcare Time Series},
  author    = {Cai, Zi and Liu, Yu and Zhu, Tingting},
  publisher   = {Preprints}
  year      = {2026},
}
```

---

## Review Structure

<details>
<summary><b>1. Introduction</b></summary>

- Search Strategy
</details>

<details>
<summary><b>2. Theoretical Foundation</b></summary>

- 2.1 Problem Categorization
- 2.2 Formalization and Notation
- 2.3 The Challenge of Time-Dependent Confounding
- 2.4 Identifiability of Time-Varying ITE
</details>

<details>
<summary><b>3. From Theory to Practice</b></summary>
</details>

<details>
<summary><b>4. Time-Varying ITE Estimation Methodology</b></summary>

- 4.1 Matching
- 4.2 G-Formula
- 4.3 Inverse Probability of Treatment Weighting
- 4.4 Representation Balancing
  - 4.4.1 Predictive Balancing
  - 4.4.2 Distribution Alignment
- 4.5 Representation Disentanglement
</details>

<details>
<summary><b>5. Clinical Application Scenarios</b></summary>

- Critical Care
- Secondary Care
- Public Health
</details>

<details>
<summary><b>6. Evaluation</b></summary>

- 6.1 Datasets
  - 6.1.1 Synthetic Datasets
  - 6.1.2 Semi-Synthetic Datasets
  - 6.1.3 Real-World Datasets
- 6.2 Evaluation Metrics
  - 6.2.1 Outcome Prediction
  - 6.2.2 Treatment Prediction
  - 6.2.3 Treatment Effect Estimation
  - 6.2.4 Representation Evaluation
- 6.3 Baselines
</details>

<details>
<summary><b>7. Current Challenges</b></summary>

- 7.1 Challenges From Data
  - 7.1.1 Continuous Time Dynamics
  - 7.1.2 Irregularities
- 7.2 Evaluation Challenges
  - 7.2.1 Unobservable Counterfactuals
  - 7.2.2 Reproducibility
</details>

<details>
<summary><b>8. Future Directions</b></summary>

- 8.1 Time-to-Event Outcomes in Time-Varying ITE
- 8.2 Multi-Modality for Time-Varying ITE
- 8.3 Digital Twin in Time-Varying ITE
</details>

<details>
<summary><b>9. Conclusion</b></summary>
</details>

---

## Methods

> **This is an updating list.** It includes deep learning methods for time-varying ITE estimation evaluated on healthcare data, ordered chronologically by publication year.

Column definitions:
- **Year**: Publication year.
- **Method**: Method name or abbreviation as used in the literature.
- **Reference**: First author(s) of the paper.
- **Venue**: Publication venue (conference or journal abbreviation).
- **Paper**: Link to the paper (arXiv preprint, publisher page, or DOI).
- **Repo**: Link to the open-source code repository, if publicly available.

| Year | Method | Reference | Venue | Paper | Repo |
|:----:|--------|-----------|-------|:-----:|:----:|
| 2018 | R-MSN | Lim | NeurIPS | [Link](https://proceedings.neurips.cc/paper/2018/hash/56e6a93212e4482d99c84a639d254b67-Abstract.html) | [Code](https://github.com/sjblim/rmsn_nips_2018) |
| 2020 | G-Net | Li et al. | ML4H | [Link](https://proceedings.mlr.press/v158/li21a) | |
| 2020 | CRN | Bica et al. | ICLR | [Link](https://arxiv.org/abs/2002.04083) | [Code](https://github.com/ioanabica/Counterfactual-Recurrent-Network) |
| 2020 | DSW | Liu et al. | ICDM | [Link](https://arxiv.org/abs/2008.13620) | [Code](https://github.com/ruoqi-liu/DSW) |
| 2021 | SyncTwin | Qian et al. | NeurIPS | [Link](https://proceedings.neurips.cc/paper/2021/hash/19485224d128528da1602ca47383f078-Abstract.html) | [Code](https://github.com/ZhaozhiQIAN/SyncTwin-NeurIPS-2021) |
| 2021 | DCRN | Berrevoets et al. | arXiv | [Link](https://arxiv.org/abs/2112.03811) | |
| 2022 | CF-ODE | De Brouwer et al. | AISTATS | [Link](https://arxiv.org/abs/2202.11987) | [Code](https://github.com/microsoft/cf-ode) |
| 2022 | CT | Melnychuk et al. | ICML | [Link](https://arxiv.org/abs/2204.07258) | [Code](https://github.com/Valentyn1997/CausalTransformer) |
| 2022 | TE-CDE | Seedat et al. | ICML | [Link](https://arxiv.org/abs/2206.08311) | [Code](https://github.com/seedatnabeel/TE-CDE) |
| 2022 | TCFimt | Xi et al. | arXiv | [Link](https://arxiv.org/abs/2212.08890) | |
| 2022 | DR-CRN | Chu et al. | CMPB | [Link](https://doi.org/10.1016/j.cmpb.2022.107175) | [Code](https://github.com/ZJU-BMI/DR-CRN) |
| 2023 | LipCDE | Cao et al. | AAAI | [Link](https://arxiv.org/abs/2303.02320) | |
| 2023 | LipSCDE | Cao et al. | arXiv | [Link](https://arxiv.org/abs/2302.09446) | |
| 2023 | SCouT | Dedhia et al. | ACM HEALTH | [Link](https://arxiv.org/abs/2207.04208) | [Code](https://github.com/JHA-Lab/scout) |
| 2023 | CF-GODE | Jiang et al. | KDD | [Link](https://arxiv.org/abs/2306.11216) | |
| 2023 | RCAB | Zhu et al. | IJCIS | [Link](https://doi.org/10.1007/s44196-023-00228-3) | |
| 2024 | T4 | Liu et al. | Nature MI | [Link](https://www.nature.com/articles/s42256-023-00638-0) | [Code](https://github.com/ruoqi-liu/T4) |
| 2024 | Su et al. | Su et al. | AMIA | [Link](https://pmc.ncbi.nlm.nih.gov/articles/PMC11141800/) | |
| 2024 | G-Transformer | Xiong et al. | CHIL | [Link](https://arxiv.org/abs/2406.05504) | |
| 2024 | G-Transformer | Hess et al. | arXiv | [Link](https://arxiv.org/abs/2405.21012) | [Code](https://github.com/konstantinhess/G_transformer) |
| 2024 | CURE | Liu et al. | Patterns | [Link](https://www.cell.com/patterns/fulltext/S2666-3899(24)00081-3) | [Code](https://github.com/ruoqi-liu/CURE) |
| 2024 | Wu et al. | Wu et al. | KDD | [Link](https://arxiv.org/abs/2305.15742) | [Code](https://github.com/ShenghaoWu/Counterfactual-Generative-Models) |
| 2024 | CAG-ODE | Huang et al. | WWW | [Link](https://arxiv.org/abs/2403.00178) | [Code](https://github.com/Jun-Kai-Zhang/CAG-ODE) |
| 2024 | ACTIN | Wang et al. | ICML | [Link](https://openreview.net/forum?id=126SR50BEL) | [Code](https://github.com/waxin/ACTIN) |
| 2024 | Causal CPC | El Bouchattaoui et al. | NeurIPS | [Link](https://arxiv.org/abs/2406.00535) | |
| 2024 | OptAB | Wendland et al. | npj Digital Medicine | [Link](https://www.nature.com/articles/s41746-024-01350-y) | [Code](https://github.com/philippwendland/OptAB) |
| 2025 | SCIP-Net | Hess and Feuerriegel | ICLR | [Link](https://arxiv.org/abs/2410.03514) | [Code](https://github.com/konstantinhess/SCIP-Net) |
| 2025 | VTDNet | Dai et al. | JBI | [Link](https://doi.org/10.1016/j.jbi.2025.104880) | [Code](https://github.com/Throwfox/VTDNet) |
| 2025 | IVW-DR-learner | Frauen et al. | ICLR | [Link](https://arxiv.org/abs/2407.05287) | [Code](https://github.com/DennisFrauen/CATEMetaLearnersTime) |
| 2025 | CEET | Zhang et al. | ISCAIT | [Link](https://ieeexplore.ieee.org/document/11010767/) | |
| 2025 | Liu et al. | Liu et al. | Preprint | [Link](https://arxiv.org/abs/2511.16006) | |
| 2025 | EDTS | Norimatsu and Imaizumi | CLeaR | [Link](https://proceedings.mlr.press/v275/norimatsu25a.html) | [Code](https://github.com/ynorimat/EDTS) |
| 2025 | Mamba-CDSP | Wang et al. | ICLR | [Link](https://openreview.net/forum?id=yheQRc5xWB) | |
| 2025 | Guski et al. | Guski et al. | Scientific Reports | [Link](https://www.nature.com/articles/s41598-025-88433-2) | [Code](https://github.com/SCAI-BIO/causal-npi-effects) |
| 2025 | TV-SurvCaus | Abraich | arXiv | [Link](https://arxiv.org/abs/2505.01785) | |
