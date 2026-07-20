<div align="center">

# FuSS-Net

### Multi-level Fusion of Frequency Priors and Semantic State Space Dynamics for Synergistic Lesion Segmentation and Classification

[![Manuscript](https://img.shields.io/badge/Manuscript-Under%20Review-orange.svg)](#citation)
[![Code](https://img.shields.io/badge/Code-Coming%20Soon-yellow.svg)](#repository-status)
[![Framework](https://img.shields.io/badge/Framework-PyTorch-EE4C2C.svg?logo=pytorch&logoColor=white)](#planned-release)
[![Task](https://img.shields.io/badge/Task-Segmentation%20%2B%20Classification-6A5ACD.svg)](#overview)
[![GitHub stars](https://img.shields.io/github/stars/Hugo271828/FuSS-Net?style=social)](https://github.com/Hugo271828/FuSS-Net)

**Official project repository for FuSS-Net**

</div>

---

## 🔍 Overview

FuSS-Net is a unified multi-task framework for **joint lesion segmentation and classification**. It formulates lesion analysis as a hierarchical information-fusion problem spanning three levels:

- **representation-level fusion:** fuzzy rule-based adaptive frequency filtering;
- **propagation-level fusion:** semantic-adaptive fuzzy-gated visual state space modeling;
- **decision-level fusion:** texture-enhanced Choquet non-additive feature aggregation.

The framework is evaluated on the **Oral Ulcer Dataset (OUD)**, **ISIC 2017**, **BUSI**, and the external **Autooral** dataset.

---

## 🧠 Architecture

<p align="center">
  <img src="assets/fussnet_framework.png" width="100%" alt="FuSS-Net architecture">
</p>

<p align="center"><em>Overall architecture of FuSS-Net. FRAF, FVSS, and TECC operate at the representation, propagation, and decision levels, respectively.</em></p>

### Core modules

| Module | Full name | Main role |
|---|---|---|
| **FRAF** | Fuzzy Rule-based Adaptive Frequency Filtering | Adaptively integrates frequency-domain priors into shallow spatial features to enhance lesion boundaries and heterogeneous textures. |
| **FVSS** | Fuzzy Visual State Space | Converts image-level category priors and token-level semantic consistency into token-wise fuzzy gates before selective scan. |
| **TECC** | Texture-Enhanced Choquet Classification | Performs non-additive fusion of frequency-enhanced shallow texture features and deep semantic representations. |

---

## ✨ Highlights

- A unified multi-level fusion framework for synergistic lesion segmentation and classification.
- Input-adaptive fuzzy frequency routing for boundary- and texture-sensitive representation learning.
- Semantic-aware fuzzy gating of state space propagation for improved cross-task coordination.
- Choquet-integral-based non-additive fusion for modeling complementary and redundant feature interactions.
- Evaluation across oral ulcer, dermoscopic, and breast ultrasound imaging scenarios, including zero-shot external validation.

---

## 📊 Main Results

The following results are reported in the manuscript as mean ± standard deviation under the corresponding evaluation protocols.

| Dataset | Evaluation setting | Seg. IoU (%) | Seg. F1 (%) | Cls. Acc. (%) | Cls. F1 (%) |
|---|---:|---:|---:|---:|---:|
| **OUD** | In-domain | **90.87 ± 0.86** | **95.22 ± 0.55** | **98.44 ± 0.22** | **98.44 ± 0.22** |
| **ISIC 2017** | In-domain | **83.50 ± 1.15** | **91.11 ± 0.96** | **86.00 ± 0.22** | **86.16 ± 0.60** |
| **BUSI** | In-domain | **68.30 ± 1.81** | **81.21 ± 2.05** | **93.59 ± 0.65** | **93.55 ± 0.54** |
| **Autooral** | Zero-shot OUD → Autooral | **48.68 ± 0.63** | **65.48 ± 0.59** | **88.09 ± 0.35** | **90.34 ± 0.06** |

**Model profile:** 29.17M trainable parameters, 8.82 GFLOPs, and 359.13 ms inference latency under the experimental setting reported in the manuscript.

---

## 🚧 Repository Status

> [!IMPORTANT]
> This repository currently serves as the official project page for FuSS-Net. The complete implementation and reproduction materials are undergoing institutional review and collaborative intellectual-property assessment.

Public release of the code is subject to:

- data-governance policies of the participating hospital;
- institutional and ethical requirements;
- patient-privacy protection;
- research and industry collaboration agreements;
- intellectual-property review.

After manuscript acceptance and completion of the required review procedures, approved code, configurations, and reproduction instructions will be released here when permitted.

Academic requests for access to approved research materials may be considered on a reasonable-request basis.

---

## 📦 Planned Release

Subject to institutional and collaborative approval, the repository is expected to provide:

- [ ] core FuSS-Net implementation;
- [ ] FRAF, FVSS, and TECC modules;
- [ ] training and evaluation scripts;
- [ ] dataset configuration examples;
- [ ] model configuration files;
- [ ] inference and metric-computation scripts;
- [ ] instructions for reproducing the main experiments;
- [ ] selected pretrained model weights, when permitted.

The final release scope may be adjusted according to institutional, ethical, and intellectual-property requirements.

---

## 🗂️ Data Availability

### Public datasets

The public datasets used in this study should be obtained from their original sources:

- **ISIC 2017**;
- **Breast Ultrasound Images Dataset (BUSI)**;
- **Autooral**.

Users are responsible for complying with the corresponding licenses and terms of use.

### Oral Ulcer Dataset

The **Oral Ulcer Dataset (OUD)** is a self-constructed clinical dataset containing oral mucosal images, lesion-category annotations, and pixel-level segmentation masks.

Because OUD contains clinical data, access is governed by institutional data-management policies, ethical approval, patient-privacy requirements, and applicable collaborative agreements. An approved version may be considered for non-commercial academic research upon reasonable request.

A request may require:

1. a description of the proposed academic use;
2. institutional affiliation and researcher information;
3. confirmation of non-commercial use;
4. completion of a data-use agreement;
5. approval from the relevant institutional and ethical authorities.

> [!NOTE]
> Access to OUD is not automatic and cannot be guaranteed.

---

## 📝 Citation

Please cite the following manuscript when using FuSS-Net or materials released through this repository:

```bibtex
@article{li_fussnet_2026,
  title   = {FuSS-Net: Multi-level Fusion of Frequency Priors and Semantic State Space Dynamics for Synergistic Lesion Segmentation and Classification},
  author  = {Li, Tianxiang and Liu, Yang and Pedrycz, Witold and Sun, Yuchun and Ding, Weiping and Tian, Sukun},
  journal = {Information Fusion},
  year    = {2026},
  note    = {Manuscript under review}
}
```

---

## 📬 Contact

For academic inquiries regarding FuSS-Net, please contact:

**Tianxiang Li**  
📧 [litianxiang20@mails.ucas.ac.cn](mailto:litianxiang20@mails.ucas.ac.cn)

When requesting research materials, please include your institutional affiliation, intended use, and a brief description of the proposed study.

---

## ⚖️ License

The code license and permitted scope of use will be specified when the approved implementation is released. Dataset access and use are governed separately by the applicable institutional, ethical, and data-use requirements.
