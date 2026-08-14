# Yoruba Language Model Fine-Tuning

## Project Overview

This project focuses on adapting and fine-tuning a pretrained language model for Yoruba language instruction-following tasks. The study explores the use of parameter-efficient fine-tuning (LoRA) to improve the model's ability to understand and generate Yoruba responses.

## Abstract

This study investigates the adaptation and fine-tuning of a pretrained language model for Yoruba language instruction-following tasks. A dataset of 3,598 Yoruba instruction-response pairs was processed using Adaption Lab and divided into 3,238 training samples and 360 validation samples. The Qwen2.5-0.5B-Instruct model was fine-tuned using Low-Rank Adaptation (LoRA) for one epoch. The model achieved a training loss of 0.4671, validation loss of 0.1161, and mean token accuracy of 95.77%. Quantitative evaluation produced a BLEU score of 4.42 and an exact-match score of 0%. Qualitative analysis identified challenges including poor instruction following, repetition, grammatical and semantic errors, and English/multilingual leakage. The findings demonstrate both the potential and limitations of fine-tuning low-resource Yoruba language models and highlight the importance of high-quality datasets and improved evaluation methods.

## Objectives

- Adapt a dataset for Yoruba language modeling.
- Fine-tune a pretrained language model for Yoruba instruction-following.
- Evaluate the performance of the fine-tuned model.
- Compare the fine-tuned model with the original base model.
- Identify common errors in Yoruba language generation.

## Dataset

The dataset contains:

- Total records: **3,598**
- Training samples: **3,238**
- Validation samples: **360**
- Language: **Yoruba**
- Task type: **Instruction-response generation**

The adapted dataset was processed using Adaption Lab.

## Model and Training

**Base model:** Qwen2.5-0.5B-Instruct

**Fine-tuning method:** Low-Rank Adaptation (LoRA)

**GPU:** NVIDIA Tesla T4

**Epochs:** 1

The fine-tuned model was trained using the Hugging Face Transformers, PEFT, TRL, and Datasets libraries.

## Results

| Metric | Result |
|---|---:|
| Dataset size | 3,598 |
| Training samples | 3,238 |
| Validation samples | 360 |
| Epochs | 1 |
| Training loss | 0.4671 |
| Validation loss | 0.1161 |
| Mean token accuracy | 95.77% |
| BLEU | 4.42 |
| Exact Match | 0% |

## Qualitative Evaluation

The fine-tuned model was evaluated using Yoruba prompts covering tasks such as:

- Sentence negation
- Question formation
- Yoruba grammar explanation
- Yoruba sentence generation
- Sports-related sentences

The evaluation showed that the model was able to produce Yoruba text but still experienced several generation problems.

## Error Analysis

The major error categories observed were:

1. **Wrong Yoruba response** – expected grammatical or task-specific responses were not consistently produced.
2. **Poor instruction following** – the model sometimes repeated the prompt rather than answering it.
3. **English/multilingual leakage** – English and other languages appeared in some outputs.
4. **Repetition** – some responses contained repeated phrases.
5. **Grammatical and semantic errors** – some generated sentences were fragmented or semantically incorrect.

## Training Loss

The training-loss graph generated during fine-tuning is available in:

`training_loss_graph.png`

## Project Files

- `*.ipynb` – Google Colab notebook containing the implementation and experiments.
- `yoruba_focus_nlp.json` – Yoruba dataset used in the project.
- `training_loss_graph.png` – Training performance visualization.
- `README.md` – Project documentation.

## Technologies Used

- Python
- Google Colab
- PyTorch
- Hugging Face Transformers
- Hugging Face Datasets
- PEFT
- TRL
- LoRA
- Adaption Lab

## Conclusion

The experiment demonstrates the feasibility of fine-tuning a small pretrained language model for Yoruba instruction-following tasks. Although the model achieved a high mean token accuracy during training, the relatively low BLEU score and 0% exact match indicate that further improvements are required. Future work should focus on improving dataset quality, increasing the number of training epochs, expanding evaluation datasets, and exploring additional Yoruba-specific language resources.

## Author

**Kolawole Joseph Tayo and Mariam Olodude**

Linguistics Island

## Acknowledgement

This project was developed as part of practical work in computational linguistics and natural language processing, with a focus on low-resource Yoruba language technology.
