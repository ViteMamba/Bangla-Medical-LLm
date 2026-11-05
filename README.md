# Bengali Medical LLM — QLoRA Fine-tuning

## Project Overview
Fine-tuning TigerLLM-1B-it (Gemma3) on Bengali medical QA dataset
using QLoRA for resource-efficient domain adaptation.

## Model
- Base: md-nishat-008/TigerLLM-1B-it
- Architecture: Gemma3
- Fine-tuned: Shakil2448868/TigerLLM-Medical-Bengali

## Dataset
- Shakil2448868/Bangla-medical-question-answering
- 901 samples, Bengali medical QA with Chain-of-Thought

## Method
- QLoRA (4-bit quantization + LoRA adapters)
- LoRA rank: r=16, alpha=32
- GPU: Tesla T4 (Kaggle free tier)

## Results
| Metric  | Base Model | Fine-tuned |
|---------|-----------|------------|
| ROUGE-1 | TBD       | TBD        |
| ROUGE-L | TBD       | TBD        |
| BLEU    | TBD       | TBD        |

## How to Run
```bash
pip install -r requirements.txt
# Open notebook.ipynb in Kaggle
```

## Demo
HuggingFace Space: https://huggingface.co/spaces/Shakil2448868/TigerLLM-Medical-Bengali