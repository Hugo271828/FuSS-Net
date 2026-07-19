# FuSS-Net

Official repository for:

**FuSS-Net: Multi-level Fusion of Frequency Priors and Semantic State Space Dynamics for Synergistic Lesion Segmentation and Classification**

FuSS-Net is a joint lesion segmentation and classification framework that integrates:

- fuzzy rule-based adaptive frequency filtering;
- semantic-adaptive fuzzy-gated visual state space propagation;
- texture-enhanced Choquet non-additive feature fusion.

The framework is evaluated on the Oral Ulcer Dataset (OUD), ISIC 2017, BUSI, and the external Autooral dataset.

---

## Repository Status

This repository currently serves as the official project page for FuSS-Net.

The core implementation and reproduction materials are undergoing institutional review and collaborative intellectual-property assessment. Public release of the complete code is subject to the data-governance policies of the participating hospital, ethical requirements, and the terms of the relevant research and industry collaboration agreements.

After manuscript acceptance and completion of the required review procedures, the approved core code, configuration files, and reproduction instructions will be released in this repository when permitted.

Academic requests for access to approved research materials may be considered on a reasonable-request basis.

---

## Planned Release

Subject to institutional and collaborative approval, the repository is expected to provide:

- the core FuSS-Net model implementation;
- FRAF, FVSS, and TECC module implementations;
- training and evaluation scripts;
- dataset configuration examples;
- model configuration files;
- inference and metric-computation scripts;
- instructions for reproducing the main experiments;
- selected pretrained model weights, when permitted.

The exact release scope may be adjusted according to institutional, ethical, and intellectual-property requirements.

---

## Data Availability

### Public datasets

The public datasets used in this study are available from their original sources:

- ISIC 2017;
- Breast Ultrasound Images Dataset (BUSI);
- Autooral.

Users should obtain these datasets directly from their official sources and comply with the corresponding licenses and terms of use.

### Oral Ulcer Dataset

The Oral Ulcer Dataset (OUD) is a self-constructed clinical dataset containing oral mucosal images, lesion-category annotations, and pixel-level segmentation masks.

Because the dataset involves clinical data, access is governed by institutional data-management policies, ethical approval, patient-privacy requirements, and applicable collaborative agreements. An approved version of the dataset may be made available for non-commercial academic research upon reasonable request, subject to institutional and ethical review.

Access to OUD is therefore not guaranteed automatically and may require:

1. a description of the proposed academic use;
2. institutional affiliation and researcher information;
3. confirmation of non-commercial use;
4. completion of a data-use agreement;
5. approval from the relevant institutional and ethical authorities.

---

## Citation

If you use FuSS-Net or materials released through this repository, please cite:

```bibtex
@article{li_fussnet_2026,
  title   = {FuSS-Net: Multi-level Fusion of Frequency Priors and Semantic State Space Dynamics for Synergistic Lesion Segmentation and Classification},
  author  = {Li, Tianxiang and Liu, Yang and Pedrycz, Witold and Sun, Yuchun and Ding, Weiping and Tian, Sukun},
  journal = {Information Fusion},
  year    = {2026},
  note    = {Manuscript under review}
}
