# Natural Language Understanding of Devanagari Script Languages - CHIPSAL@COLING 2025

This repository contains our implementation for the Shared Task on Natural Language Understanding of Devanagari Script Languages, organized as part of CHIPSAL@COLING 2025. This task focuses on addressing key challenges in processing Devanagari-scripted languages through three subtasks: language identification, hate speech detection, and target identification for hate speech.

---

## Paper Abstract

Text-based hate speech has been prevalent and is usually used to incite hostility and violence. Detecting this content becomes imperative, yet the task is challenging, particularly for low-resource languages in the Devanagari script, which must have the extensive labeled datasets required for effective machine learning. To address this, a shared task has been organized for identifying hate speech targets in Devanagari-script text. The task involves classifying targets such as individuals, organizations, and communities and identifying different languages within the script. We have explored several machine learning methods such as LR, SVM, MNB, and Random Forest, deep learning models using CNN, BiLSTM, GRU, CNN+BiLSTM, and transformer-based models like Indic-BERT, m-BERT, Verta-BERT, XLM-R, and MuRIL. The CNN with BiLSTM yielded the best performance (F1-score of 0.9941), placing the team 13th in the competition for script identification. Furthermore, the fine-tuned MuRIL-BERT model resulted in an F1 score of 0.6832, ranking us 4th for detecting hate speech targets.

--- 

- To cite this paper, please use following `bibtex` command.

```
@inproceedings{hossan-etal-2025-cuet,
    title = "{CUET}{\_}{B}ig{\_}{O}@{NLU} of {D}evanagari Script Languages 2025: Identifying Script Language and Detecting Hate Speech Using Deep Learning and Transformer Model",
    author = "Hossan, Md. Refaj  and
      Sakib, Nazmus  and
      Miah, Md. Alam  and
      Hossain, Jawad  and
      Hoque, Mohammed Moshiul",
    editor = "Sarveswaran, Kengatharaiyer  and
      Vaidya, Ashwini  and
      Krishna Bal, Bal  and
      Shams, Sana  and
      Thapa, Surendrabikram",
    booktitle = "Proceedings of the First Workshop on Challenges in Processing South Asian Languages (CHiPSAL 2025)",
    month = jan,
    year = "2025",
    address = "Abu Dhabi, UAE",
    publisher = "International Committee on Computational Linguistics",
    url = "https://aclanthology.org/2025.chipsal-1.27/",
    pages = "253--259",
    abstract = "Text-based hate speech has been prevalent and is usually used to incite hostility and violence. Detecting this content becomes imperative, yet the task is challenging, particularly for low-resource languages in the Devanagari script, which must have the extensive labeled datasets required for effective machine learning. To address this, a shared task has been organized for identifying hate speech targets in Devanagari-script text. The task involves classifying targets such as individuals, organizations, and communities and identifying different languages within the script. We have explored several machine learning methods such as LR, SVM, MNB, and Random Forest, deep learning models using CNN, BiLSTM, GRU, CNN+BiLSTM, and transformer-based models like Indic-BERT, m-BERT, Verta-BERT, XLM-R, and MuRIL. The CNN with BiLSTM yielded the best performance (F1-score of 0.9941), placing the team 13th in the competition for script identification. Furthermore, the fine-tuned MuRIL-BERT model resulted in an F1 score of 0.6832, ranking us 4th for detecting hate speech targets."
}
```


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
To see overall working procedure, please visit here [link](https://aclanthology.org/2025.chipsal-1.27/)

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
