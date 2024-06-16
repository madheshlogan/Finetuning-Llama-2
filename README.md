# Finetuning-Llama-2
# LLaMA Fine-Tuning

This repository contains code and configuration files for fine-tuning the [LLaMA](https://huggingface.co/NousResearch/Llama-2-7b-chat-hf) (Large Language Model from Anthropic) using the [PEFT](https://github.com/huggingface/peft) (Parameter-Efficient Fine-Tuning) library and other optimization techniques.

## Overview

The goal of this project is to fine-tune the LLaMA-2-7B model on a specific dataset (`mlabonne/guanaco-llama2-1k`) using efficient fine-tuning techniques like QLoRA (Quantized Low-Rank Attention) and bitsandbytes quantization. These techniques aim to reduce the memory footprint and computational requirements, making it possible to fine-tune large language models on modest hardware.

## Features

- Fine-tuning the LLaMA-2-7B model using the `mlabonne/guanaco-llama2-1k` dataset
- Parameter-efficient fine-tuning with QLoRA (Quantized Low-Rank Attention)
- Memory optimization with bitsandbytes quantization (4-bit precision and nested quantization)
- Mixed-precision training (FP16 or BF16)
- Gradient checkpointing for reduced memory usage
- Learning rate scheduling (cosine)
- Gradient clipping for stability
- Checkpointing and logging during training
