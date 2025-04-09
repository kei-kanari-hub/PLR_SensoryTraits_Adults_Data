# README – PLR_SensoryTraits_Adults_Data

## Dataset Version  
Created on: 2025-04-09

---

## Title  
**Do Dynamic Pupillary Light Reflex Parameters Reflect and Predict Sensory Traits?**  
Multivariate and Machine Learning Evidence in Adults

---

## Description  
This dataset accompanies a study investigating whether dynamic pupillary light reflex (PLR) parameters reflect and predict sensory processing traits in adults.

It includes:
- Summary-level PLR indices extracted from pupil recordings
- Self-report questionnaire scores related to neurodevelopmental and sensory processing traits

All PLR indices were computed from raw pupil diameter data recorded at 500 Hz using a controlled light stimulation protocol. Questionnaire scores were obtained using Japanese-validated versions of standardized psychometric instruments.

**Note:**  
Each row represents a single participant. No personal identifiers are included.
---

## File Overview

### `dataset.csv`  
A CSV file with one row per participant and one column per variable. No ID column is included.

| Column name     | Description                                                                |
|-----------------|----------------------------------------------------------------------------|
| sex             | Biological sex: `0` = male, `1` = female                                   |
| age             | Age in years                                                               |
| AQ              | Autism Spectrum Quotient score                                             |
| ASRS Part A     | Adult ADHD Self-Report Scale Part A score                                  |
| ASRS Total      | Total ASRS score (Part A + B)                                              |
| AASP R          | AASP: Low Registration subscale                                            |
| AASP K          | AASP: Sensory Seeking subscale                                             |
| AASP S          | AASP: Sensory Sensitivity subscale                                         |
| AASP A          | AASP: Sensory Avoiding subscale                                            |
| Taste/smell     | Sensory traits score (taste/smell modality)                                |
| Movement        | Sensory traits score (movement modality)                                   |
| Visual          | Sensory traits score (visual modality)                                     |
| Touch           | Sensory traits score (tactile modality)                                    |
| Activity level  | Behavioral modulation of activity level                                    |
| Auditory        | Sensory traits score (auditory modality)                                   |
| A-State         | State anxiety score (STAI)                                                 |
| A-Trait         | Trait anxiety score (STAI)                                                 |
| TL_W            | Pupil latency (white light condition)                                      |
| Tc_R            | Constriction time (red light)                                              |
| Tr_G            | Recovery time (green light)                                                |
| Vc_B            | Constriction velocity (blue light)                                         |
| Vr_W            | Recovery velocity (white light)                                            |
| A_B             | Relative constriction amplitude (blue light)                               |
| ...             | Additional PLR parameters (see manuscript for details)                     |

**Data quality:**  
- All columns contain numeric values only.

---

## Licensing  
This dataset is released under the **CC0 1.0 Universal Public Domain Dedication**.  
You are free to copy, modify, distribute, and use the data for any purpose, without permission or attribution.

🔗 [https://creativecommons.org/publicdomain/zero/1.0/](https://creativecommons.org/publicdomain/zero/1.0/)

---

## Citation  
If you use this dataset, please cite the following paper (in preparation):

> *Do Dynamic Pupillary Light Reflex Parameters Reflect and Predict Sensory Traits? Multivariate and Machine Learning Evidence in Adults.*

---

## Contact  
**Kei Kanari**  
Tohoku University  
📧 kei.kanari.a2@tohoku.ac.jp
