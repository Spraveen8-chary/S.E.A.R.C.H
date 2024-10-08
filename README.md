# S.E.A.R.C.H : Systematic Engine for Analyzed Retrieval and Contextual Handling

![](assets/banner.png)

## Table of Contents

- [S.E.A.R.C.H : Systematic Engine for Analyzed Retrieval and Contextual Handling](#search--systematic-engine-for-analyzed-retrieval-and-contextual-handling)
  - [Table of Contents](#table-of-contents)
  - [Introduction](#introduction)
  - [Installation](#installation)
  - [Usage](#usage)
    - [For local machine](#for-local-machine)
  - [Demo](#demo)

## Introduction

S.E.A.R.C.H (Systematic Engine for Analyzed Retrieval and Contextual Handling) is an advanced, multi-faceted information retrieval system backed by [Zephyr-7B](https://huggingface.co/HuggingFaceH4/zephyr-7b-beta). It integrates a Language Model with internet access for real-time, factual data acquisition, and employs a highly scalable Retrieval Augmented Generation (RAG) framework for efficient vector database processing. The application uniquely supports querying visual data, including images, and enhances reasoning through an embedded code interpreter. An innovative in-house sub-query engine significantly reduces hallucinations, ensuring precise, context-sensitive, and reliable responses

## Installation

1. Clone repo and install dependencies

```bash
git clone https://github.com/Spraveen8-chary/S.E.A.R.C.H.git
cd S.E.A.R.C.H
```

```bash
pip install -r requirements.txt
```

2. Get API keys from [SerpAPI](https://serpapi.com/) and [Cohere](https://dashboard.cohere.com/)

## Usage

- Below attached is a quickstart notebook to try it on Google Colab
  - [![Open in colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/gist/Spraveen8-chary/0f3e645ce18d4966494a7bb6052a6dd0/quick_start.ipynb)

### For local machine

Run the following command inside terminal

```bash
export SERP_API=<SERP API KEY>
export COHERE_API=<COHERE API KEY>
```

Run the gradio interface

```bash
python app.py
```

If you want to adjust parameters in `config.py`

```bash
!python app.py --retriver_top_k 25 --reranker_top_k 10 --node_chunk_size 8000
```

## Demo

https://github.com/user-attachments/assets/2e01d28e-10c9-4d0c-9349-f8820e6b7474





