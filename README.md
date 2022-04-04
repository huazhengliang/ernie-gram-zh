---
language: zh
---

# ERNIE-Gram-zh

## Introduction

ERNIE-Gram: Pre-Training with Explicitly N-Gram Masked Language Modeling for Natural Language Understanding

More detail: https://arxiv.org/abs/2010.12148

## Released Model Info

|Model Name|Language|Model Structure|
|:---:|:---:|:---:|
|ernie-gram-zh| Chinese |Layer:12, Hidden:768, Heads:12|

This released Pytorch model is converted from the officially released PaddlePaddle ERNIE model and 
a series of experiments have been conducted to check the accuracy of the conversion.

- Official PaddlePaddle ERNIE repo: https://github.com/PaddlePaddle/ERNIE
- Pytorch Conversion repo:  https://github.com/nghuyong/ERNIE-Pytorch

## How to use
```Python
from transformers import AutoTokenizer, AutoModel
tokenizer = AutoTokenizer.from_pretrained("nghuyong/ernie-gram-zh")
model = AutoModel.from_pretrained("nghuyong/ernie-gram-zh")
```