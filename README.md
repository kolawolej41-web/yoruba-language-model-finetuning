# Yoruba Qwen Fine-Tuned Model

## Overview

This model is a LoRA fine-tuned version of **Qwen2.5-0.5B-Instruct** developed for Yoruba language instruction-following tasks.

The project explores the use of parameter-efficient fine-tuning for **low-resource African language NLP**, with a particular focus on Yoruba.

## Dataset

The dataset was adapted using **Adaption Lab** and contains:

- Total records: 3,598
- Training samples: 3,238
- Validation samples: 360
- Language: Yoruba
- Task: Instruction-response generation

## Fine-Tuning

- Base model: Qwen2.5-0.5B-Instruct
- Method: LoRA (Low-Rank Adaptation)
- Epochs: 1
- GPU: NVIDIA Tesla T4
- Platform: Google Colab

## Results

| Metric | Result |
|---|---:|
| Training Loss | 0.4671 |
| Validation Loss | 0.1161 |
| Mean Token Accuracy | 95.77% |
| BLEU | 4.42 |
| Exact Match | 0% |

## Evaluation

The model was evaluated using Yoruba prompts involving:

- Sentence negation
- Question formation
- Yoruba grammar explanation
- Yoruba sentence generation

The evaluation showed that the model could generate Yoruba-related text but still experienced challenges with instruction following, repetition, grammatical and semantic errors, and multilingual leakage.

## Limitations

The model is an experimental research model and should not be considered a fully reliable Yoruba language assistant. The low BLEU score and 0% Exact Match indicate that further improvement is required.

Future work should include higher-quality Yoruba instruction data, more training, larger evaluation sets, and improved Yoruba-specific evaluation methods.

## Tools Used

- Python
- Google Colab
- PyTorch
- Hugging Face Transformers
- Hugging Face Datasets
- PEFT
- TRL
- LoRA
- Adaption Lab

## Author

**Kolawole Joseph Tayo ansd # Yoruba Qwen Fine-Tuned Model

## Overview

This model is a LoRA fine-tuned version of **Qwen2.5-0.5B-Instruct** developed for Yoruba language instruction-following tasks.

The project explores the use of parameter-efficient fine-tuning for **low-resource African language NLP**, with a particular focus on Yoruba.

## Dataset

The dataset was adapted using **Adaption Lab** and contains:

- Total records: 3,598
- Training samples: 3,238
- Validation samples: 360
- Language: Yoruba
- Task: Instruction-response generation

## Fine-Tuning

- Base model: Qwen2.5-0.5B-Instruct
- Method: LoRA (Low-Rank Adaptation)
- Epochs: 1
- GPU: NVIDIA Tesla T4
- Platform: Google Colab

## Results

| Metric | Result |
|---|---:|
| Training Loss | 0.4671 |
| Validation Loss | 0.1161 |
| Mean Token Accuracy | 95.77% |
| BLEU | 4.42 |
| Exact Match | 0% |

## Evaluation

The model was evaluated using Yoruba prompts involving:

- Sentence negation
- Question formation
- Yoruba grammar explanation
- Yoruba sentence generation

The evaluation showed that the model could generate Yoruba-related text but still experienced challenges with instruction following, repetition, grammatical and semantic errors, and multilingual leakage.

## Limitations

The model is an experimental research model and should not be considered a fully reliable Yoruba language assistant. The low BLEU score and 0% Exact Match indicate that further improvement is required.

Future work should include higher-quality Yoruba instruction data, more training, larger evaluation sets, and improved Yoruba-specific evaluation methods.

## Tools Used

- Python
- Google Colab
- PyTorch
- Hugging Face Transformers
- Hugging Face Datasets
- PEFT
- TRL
- LoRA
- Adaption Lab

## Author

**Kolawole Joseph Tayo and Mariam Adebukola Olodude**  
Linguistics Island

## Acknowledgement

Special appreciation to **Adaption Lab** for providing a practical environment for adapting the Yoruba dataset used in this project.

This work contributes to ongoing efforts toward better representation of African languages in artificial intelligence and natural language processing.**  
Linguistics Island
## Acknowledgement

Special appreciation to **Adaption Lab** for providing a practical environment for adapting the Yoruba dataset used in this project.

This work contributes to ongoing efforts toward better representation of African languages in artificial intelligence and natural language processing.
