# Data Generation
We need to generate data to train instruction following model for sanskrit.

We will aim at following datasets:

## 1. Alpaca Data
We will translate the [cleaned alpaca dataset](https://github.com/gururise/AlpacaDataCleaned) into sanskrit using gpt4

## 2. Self Instruct Data
We will create a dataset by using data generation pipeline from [self-instruct paper](https://arxiv.org/abs/2212.10560) and [Stanford Alpaca](https://github.com/tatsu-lab/stanford_alpaca).

### 3. Self Chat

We will also generate multi-turn dialogues between human and AI assistant by using a topic and letting chatgpt generate a conversion. We can try mistral moe for this as well.


### 4. Orca-style Data
We will also generate data in the style of [Orca]() which introduces explanatory signals from the teacher model gpt-4, showcasing its reasoning process during response generation. Additionally, responses can also be generated using gpt-3.5-turbo as an intermediate teacher for curriculum learning.