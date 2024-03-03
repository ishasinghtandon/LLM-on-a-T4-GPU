# LLM-on-a-T4-GPU

# ML Engineer Assignment

## Premise
LLMs, while useful for solving various NLP related use-cases, are costly and cumbersome to productionize.
Organisations use expensive A100/H100 GPUs to deploy LLMs while extracting underwhelming performance in terms of latency and throughput.

## Problem statement
Design and develop a novel, generalised model optimisation and inference script for `MistralForCausalLM` based LLMs that:
1. Accepts a Huggingface model path as an input (example: `mistralai/Mistral-7B-v0.1`)
2. Optimises the model for faster inference (including warmups etc.)
3. Waits for user to input the prompt
4. Runs the model on the prompt
5. Outputs the model response and performance metrics

### Baseline benchmarks
Develop the script to beat the following benchmarks with the set constraints:

```Total throughput (in + out tokens per second) = 200 tokens/sec```

Here are the other details:
1. Input tokens = 128
2. Output tokens = 128
3. Concurrency = 32
4. GPU = 1 X Nvidia Tesla T4 (16GB VRAM)
5. Model dtype = any dtype of choice supported by said GPU

## Bonus
Make the script compatible with LoRA models

## Tools that offer free T4 GPUs
1. Google Colab
2. Kaggle
3. Amazon Sagemaker Studio Labs

For any clarifications, contact devansh@simplismart.ai or daksh.goel@simplismart.tech
