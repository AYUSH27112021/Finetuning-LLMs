# Fine-tuning LLM with LoRA (Low-Rank Adaptation)

LoRA (Low-Rank Adaptation) is the most used parameter-efficient fine-tuning (PEFT) method today.

This example shows you [LoRA (Low-Rank Adaptation)](https://arxiv.org/abs/2106.09685) implementation from scratch (manually) in a step-by-step manner (without ```PEFT``` package), and also shows you clear ideas behind this implementation in IPython notebook.


| Example                                                              | Description                                                             |
| -------------------------------------------------------------------- | ----------------------------------------------------------------------- |
| [01-finetune-opt-with-lora.ipynb](01-finetune-opt-with-lora.ipynb)   | Fine-tuning Meta's OPT-125M with LoRA<br>(Also, explaining LoRA method) |
| [02-finetune-gpt2-with-lora.ipynb](In progress)                      | Fine-tuning OpenAI's GPT-2 small (124M) with LoRA                       |

Unlike examples in [official repository](https://github.com/microsoft/LoRA), I download pre-trained models to focus on LoRA implementation here.

> Note: In this repository, Hugging Face API is used to download pre-trained models and I then apply a regular PyTorch training loop for fine-tuning. (I don't use the blackboxed ```Trainer``` class in Hugging Face API.)

## 1. Set-up and Install

To run this example, please install prerequisite software and set up your environment.<br>
In the following setting, I have used a GPU-utilized virtual machine (VM) with the "Ubuntu Server 20.04 LTS" image in Microsoft Azure.


### Install packages

Install PyTorch, Hugging Face transformer, and other libraries as follows.

## 2. Fine-tune (Train)

Download this repository.
Run jupyter notebook.
