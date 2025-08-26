# QLoRA-for-Automated-Paper-Review-Insights
## Overview
This project explores the task of automated reviews for scientific papers.  
The goal is to evaluate whether fine tuning a LLM (Qwen3-1.7B) can produce reviews that resemble human-written ones, while outperforming a zero shot approach, highlighting paper strengths and weaknesses.  

## Dataset
- **OpenReview 2018 dataset**  
- Around 4,700 reviews for 1,500 papers  
- Each review includes a score from 1 to 10

## Methodology
- Fine-tuned Qwen-3 1.7B with QLoRA 
- Compared against:
  - Zero-shot baseline
  - Human-written reviews

## Evaluation Metrics
- **ROUGE** (1, 2, L) – n-gram overlap with human reviews  
- **BERTScore (RoBERTa)** – semantic similarity  
- **Perplexity** – fluency and language quality  

## Results
- QLoRA outperforms zero-shot across most metrics  
- Perplexity reduced by almost 50% compared to zero-shot  
- Reviews capture key strengths and weaknesses, but they show inconsistencies  

## Conclusion
QLoRA fine-tuning shows strong potential for assisting in the peer review process, producing reviews closer to human quality than zero-shot models. While not yet a replacement for reviewers, it represents a step toward scalable, AI-assisted peer review.  

