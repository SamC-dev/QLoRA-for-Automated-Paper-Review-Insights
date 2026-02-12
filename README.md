# QLoRA-for-Automated-Paper-Review-Insights
## Overview
This project explored the task of automated reviews for scientific papers.  
The goal was to evaluate whether fine tuning a LLM (Qwen3-1.7B) can produce reviews that resemble human written ones, while outperforming a zero shot approach, highlighting paper strengths and weaknesses. Relevance was also given to the role of a good prompting strategy. 

## Dataset
- **OpenReview 2018 dataset**  
- Around 4,700 reviews for 1,500 papers  
- Final cleaned dataset of around 1500 entries

## Methodology
- Fine-tuned Qwen-3 1.7B with QLoRA 
- Compared against:
  - Zero-shot baseline
  - Human-written reviews
- Both baseline and fine tuned model tested with two system prompts: linear and few shot CoT

## Evaluation Metrics
- **ROUGE** (1, 2, L) – n-gram overlap with human reviews  
- **BERTScore (RoBERTa)** – semantic similarity  
- **Perplexity** – fluency and language quality  

## Results
- QLoRA outperforms baseline in linguistic fluency
- CoT outperforms linear prompt in baseline model 
- Reviews capture key strengths and weaknesses, but they show inconsistencies  

