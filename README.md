# Natural Language Understanding of Devanagari Script Languages - CHIPSAL@COLING 2025

This repository contains our implementation for the **Shared Task on Natural Language Understanding of Devanagari Script Languages**, organized as part of **CHIPSAL@COLING 2025**. This task focuses on addressing key challenges in processing Devanagari-scripted languages through three subtasks: language identification, hate speech detection, and target identification for hate speech.

## Task Overview

The shared task challenges participants to develop robust systems for understanding Devanagari-scripted languages across three subtasks:

### Subtask A: Devanagari Script Language Identification
- **Objective**: Classify sentences in Devanagari script into one of the following languages:
  - **Nepali**
  - **Marathi**
  - **Sanskrit**
  - **Bhojpuri**
  - **Hindi**
- **Dataset**: Sentences in Devanagari script.
- **Evaluation Metric**: Accuracy.

### Subtask B: Hate Speech Detection
- **Objective**: Detect whether a given sentence in Devanagari script contains hate speech.
- **Languages**: Nepali and Hindi.
- **Dataset**: Monolingual sentences annotated for hate speech presence.
- **Evaluation Metric**: Macro F1 Score.

### Subtask C: Targets of Hate Speech Identification
- **Objective**: Identify the target of hate speech in a hateful sentence, categorized as:
  - **Individual**
  - **Organization**
  - **Community**
- **Dataset**: Sentences annotated with hate speech targets.
- **Evaluation Metric**: Macro F1 Score.

For more details, visit [here](https://codalab.lisn.upsaclay.fr/competitions/20000).

## Repository Structure

```plaintext
├── data/
│   ├── train/                # Training data for all subtasks
│   ├── valid/                # Validation data for all subtasks
│   ├── test/                 # Test data for all subtasks
├── notebooks/
│   ├── Subtask_A_Notebook.ipynb
│   ├── Subtask_B_Notebook.ipynb
│   ├── Subtask_C_Notebook.ipynb
├── requirements.txt          # Required Python libraries
├── README.md                 # Project documentation
```

## Methodology
This section will be updated soon with details on our approach for each subtask.

### Installation
Clone the repository:
```
  git clone https://github.com/RJ-Hossan/CHIPSAL-25
  cd CHIPSAL-25
```

### Install dependencies:
```
    pip install -r requirements.txt
```
Download the datasets from [this link](https://codalab.lisn.upsaclay.fr/competitions/20000) and place them in the data/ directory.

## Acknowledgments
We thank the organizers of CHIPSAL@COLING 2025 for providing the datasets and hosting this important shared task. We also acknowledge the support of the open-source community for tools like PyTorch, Hugging Face Transformers, and Scikit-learn.
