# Fine-Tuning GPT-3.5 and LLaMA for Job Interview Preparation

This project demonstrates the fine-tuning of advanced language models, **GPT-3.5-Turbo** and **LLaMA**, on a dataset of job interview questions and answers tailored for software engineering roles. The goal is to build a conversational AI system capable of simulating realistic job interviews while evaluating technical and soft skills.

---

## Features
- **Fine-Tuning GPT-3.5 and LLaMA**: Both models are fine-tuned to generate domain-specific responses to interview questions.
- **Dataset Preparation**: Includes data cleaning, tokenization, and structuring for Natural Language Processing (NLP) tasks.
- **Performance Metrics**: Evaluates models using ROUGE and BERTScore metrics before and after optimization.
- **Model Optimization**: Implements optimization techniques to enhance performance.

---

## Requirements

### Python Libraries
- `openai`: For GPT-3.5 API integration.
- `unsloth`: For efficient fine-tuning of LLaMA.
- `tiktoken`: For token counting.
- `sacrebleu`, `rouge-score`, `bert-score`: For performance evaluation.
- `matplotlib`: For visualizing performance metrics.
- `torch`: For training and deploying the models.


### Dataset
Source: Domain-specific interview questions and answers.
Format: JSONL file with structured input for training and evaluation.

### Workflow
1. Data Preparation:
- Load and clean the dataset.
- Tokenize and structure data for NLP tasks.
2. Model Fine-Tuning:
- Train GPT-3.5-Turbo and LLaMA on the curated dataset.
- Apply parameter-efficient fine-tuning techniques (LoRA) for LLaMA.
3. Evaluation:
- Compute performance metrics using ROUGE and BERTScore.
- Compare model performance before and after optimization.
4. Analysis:
- Visualize performance metrics and analyze trends.

  
### Key Files
1- FineTuning_GPT3.5_LLaMA_JobInterview.py:
Contains the code for data preparation, fine-tuning, evaluation, and visualization.

2- Dataset Files:
- Software_Questions_GPT.jsonl: Dataset for GPT-3.5 fine-tuning.
- Software_Questions_LLaMA.jsonl: Dataset for LLaMA fine-tuning.

### Limitations
- Performance may vary with different datasets or hyperparameters.
- LLaMA requires significant computational resources for training and fine-tuning.

### Future Work
- Explore domain-specific optimizations for additional technical fields.
- Integrate real-time evaluation capabilities for user feedback.
