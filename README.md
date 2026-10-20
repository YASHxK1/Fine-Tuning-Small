# Fine-Tuning-Small
---
# Fine-Tuning-Small

A beginner-friendly project to fine-tune a small language model for mathematical reasoning using **4 GB VRAM**.

## Model & Dataset

- **Base Model:** [Qwen2.5-0.5B-Instruct](https://huggingface.co/Qwen/Qwen2.5-0.5B-Instruct)
- **Dataset:** [GSM8K](https://huggingface.co/datasets/openai/gsm8k)
- **Fine-Tuning Method:** QLoRA (4-bit)
- **Frameworks:** PyTorch, Transformers, PEFT, TRL

## Training Configuration

| Parameter | Value |
|---|---|
| GPU VRAM | 4 GB |
| Training Samples | 2,000 |
| Epochs | 1 |
| Batch Size | 1 |
| Gradient Accumulation | 8 |
| Sequence Length | 512 |
| LoRA Rank | 8 |

## Project Goals

- Learn supervised fine-tuning (SFT).
- Fine-tune an LLM on mathematical problems.
- Optimize training for limited GPU memory.
- Compare model performance before and after fine-tuning.
- Save and reuse the trained LoRA adapter.

## Evaluation

Evaluate the original and fine-tuned models on the GSM8K test split using the same inference settings.

## License

Model and dataset usage must comply with their respective licenses.
