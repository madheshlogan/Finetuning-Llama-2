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

# Results
both are generated for same query explain transformers? 

## Old response before finetuning 
Transformers are a type of electrical device that transfers electrical energy from one circuit to another through electromagnetic induction. nobody knows for sure who invented the transformer, but it is believed to have been invented in the 1880s by a British engineer named William Thomson (later Lord Kelvin). The transformer is a passive device, meaning it doesn't consume any power to operate, and it relies on electromagnetic induction to transfer energy between two circuits.

The basic structure of a transformer consists of two coils of wire, known as the primary and secondary coils, which are wrapped around a common magnetic core. When an alternating current (AC) flows through the primary coil, it generates a magnetic field that induces an electromotive force (EMF) in the secondary coil. The EMF in the secondary
add Codeadd Markdown

## New response after finetuning

Transformers are a type of neural network architecture that is commonly used for natural language processing tasks, such as language translation, text classification, and language modeling. Transformers are based on attention mechanisms that allow the network to focus on specific parts of the input data when making predictions. This allows transformers to capture long-range dependencies in the input data, which is important for tasks such as language translation.

Transformers consist of an encoder and a decoder. The encoder takes in a sequence of tokens (e.g. words or characters) and outputs a sequence of vectors that represent the input data. The decoder takes in the output of the encoder and generates a sequence of output tokens. The decoder also has an attention mechanism that allows it to focus on specific parts of the input data when generating each output token.

Transformers are trained using a large dataset of input and output pairs
