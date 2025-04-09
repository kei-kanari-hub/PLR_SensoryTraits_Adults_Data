# README – PLR_SensoryTraits_Adults_Data

## Dataset Version  
Created on: 2025-04-09

---

## Title  
Do Dynamic Pupillary Light Reflex Parameters Reflect and Predict Sensory Traits?  
Multivariate and Machine Learning Evidence in Adults

## Description  
This dataset accompanies a study investigating whether dynamic pupillary responses reflect and predict sensory processing traits in adults.  
It contains raw time-series pupil diameter data and self-report questionnaire scores.

---

## 1. participants.xlsx  
Excel file containing demographic data and questionnaire scores for each participant.

| Column         | Description                                                                |
|----------------|----------------------------------------------------------------------------|
| ID             | Participant number (1–44); corresponds to filenames such as `sub-001`, ... |
| sex            | Biological sex: `0` = male, `1` = female                                   |
| age            | Age in years                                                               |
| AQ             | Autism Spectrum Quotient score                                             |
| ASRS Part A    | Adult ADHD Self-Report Scale Part A score                                  |
| ASRS Total     | Total ASRS score (Part A + B)                                              |
| AASP R         | AASP: Registration (low registration) subscale                             |
| AASP K         | AASP: Sensory seeking subscale                                             |
| AASP S         | AASP: Sensory sensitivity subscale                                         |
| AASP A         | AASP: Sensory avoiding subscale                                            |
| Taste/smell    | Sensory traits score (taste/smell modality)                                |
| Movement       | Sensory traits score (movement modality)                                   |
| Visual         | Sensory traits score (visual modality)                                     |
| Touch          | Sensory traits score (tactile modality)                                    |
| Activity level | Behavioral modulation of activity level                                    |
| Auditory       | Sensory traits score (auditory modality)                                   |
| A-State        | State anxiety score (State-Trait Anxiety Inventory)                        |
| A-Trait        | Trait anxiety score (State-Trait Anxiety Inventory)                        |

**Notes:**  
- All questionnaire scores are based on validated Japanese versions of the respective scales.  
- Participant IDs correspond to other files, e.g., `1.csv`, `1_c.csv`.


---

## 2. [ID].csv  
Raw time-series eye-tracking data file for participant `[ID]` (e.g., `eye_data/1.csv`).  
Each row represents one sample recorded at 500 Hz (i.e., every 2 ms).

| Column  | Description                                                                                                    |
|---------|----------------------------------------------------------------------------------------------------------------|
| time    | Timestamp from recording start (in milliseconds)                                                               |
| x       | Horizontal gaze position (in **degrees** of visual angle)                                                      |
| y       | Vertical gaze position (in **degrees** of visual angle)                                                        |
| pupil   | Pupil diameter (in **pixels**)                                                                                 |
| mode    | Recording mode indicator: `2` indicates activation of the **Head Fixed - ObjectAngle** coordinate system       |
| dio     | Synchronization signal: `7→15` indicates stimulus onset                                                        |
| pratio  | Proportion of pupil openness (0–1); represents eyelid openness                                                 |
| bink    | Blink flag: `0` = no blink, any non-zero value = blink detected                                                |

**Notes:**  
- Missing or artifacted data are represented as empty cells (i.e., blank entries).  
- `x` and `y` are in degrees of visual angle.  
- `pupil` is measured in raw pixels from the eye tracker.  
- `mode` indicates the coordinate reference system used.  
- `dio` marks stimulus onset via a transition from `7` to `15`.  
- `bink` values greater than `0` denote blink-related artifacts or events.


---

## 3. [ID]_c.csv  
Experimental condition metadata file for participant `[ID]` (e.g., `condition_data/1_c.csv`).  
Each row corresponds to one trial presented during the experiment.

| Column  | Description                                                                 |
|---------|-----------------------------------------------------------------------------|
| block   | Block number indicating the progression of experimental segments            |
| trial   | Trial number within the corresponding block                                 |
| stimuli | Light stimulus condition: `1` = white, `2` = red, `3` = green, `4` = blue   |

**Notes:**  
- Trials are grouped into blocks, and ordered by their presentation within each block.  
- `stimuli` codes represent different luminance-modulated color conditions.

---

## General Notes  
- All data are anonymized and labeled with pseudo-identifiers (e.g., `1.csv`, `1_c.csv`).  
- No preprocessing (e.g., blink/saccade artifact removal) has been applied.  
- Time-series data were sampled at 500 Hz (i.e., every 2 ms).  
- All files are encoded in UTF-8 and comma-separated (`.csv`).

---

## Citation  
If you use this dataset, please cite:  
**"Do Dynamic Pupillary Light Reflex Parameters Reflect and Predict Sensory Traits? Multivariate and Machine Learning Evidence in Adults"** (in preparation)

---

## Contact:  
Kei Kanari  
Tohoku University  
Email: kei.kanari.a2@tohoku.ac.jp
