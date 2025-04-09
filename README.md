# Prompt Injection Detection using Deep Learning

[![Python](https://img.shields.io/badge/Python-3.x-blue.svg)](https://www.python.org/)
[![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x-orange.svg)](https://www.tensorflow.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
<a target="_blank" href="https://colab.research.google.com/github/https://colab.research.google.com/drive/1KKSEmB7aV2VmRNNYrsNFIUaF8Sjy9jt-?usp=sharing">
<img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
</a>

**A deep learning-based project for detecting malicious prompt injection attempts in text.**

All metrics are included in the Colab link and Jupyter notebook.

## Overview

This project implements a text classification model using TensorFlow and Keras to identify whether a given text input is a benign user prompt or an attempt to perform a prompt injection attack. Prompt injection is a security vulnerability that can allow malicious actors to manipulate the behavior of large language models (LLMs) by crafting specific input prompts that override intended instructions or extract sensitive information.

This repository contains the code for:

- Loading and preprocessing text data.
- Building and training a deep learning model (currently using an LSTM-based architecture).
- Evaluating the model's performance on validation and test datasets.
- Making predictions on new, unseen text.
- Generating a confusion matrix and classification report for evaluation.

## Why Prompt Injection Detection is More Important Now Than Ever Before

The rise and widespread adoption of Large Language Models (LLMs) have brought unprecedented capabilities in various applications, from content generation and chatbots to code completion and research assistance. However, this powerful technology also introduces new security challenges, and **prompt injection stands out as a critical vulnerability that demands immediate attention.**

Here's why prompt injection detection is more important now than ever before:

- **Increased Reliance on LLMs:** As LLMs become increasingly integrated into everyday applications and critical infrastructure, the potential impact of successful prompt injection attacks grows exponentially. Compromising an LLM can lead to the manipulation of downstream systems, data breaches, the spread of misinformation, and reputational damage.

- **Circumventing Guardrails:** Many LLM providers implement safety guidelines and filters. However, prompt injection techniques can often be used to circumvent these guardrails, allowing malicious actors to generate harmful content, bypass ethical restrictions, or elicit biased responses that the LLM was designed to avoid.

- **Data Exfiltration and System Compromise:** Successful prompt injections can be leveraged to extract sensitive information that the LLM has access to or is connected to. In more severe cases, if the LLM has access to external tools or APIs, prompt injection could potentially lead to the compromise of underlying systems.

- **Scalability of the Threat:** LLMs are designed to process vast amounts of user input. This scalability also applies to potential attacks. A single well-crafted injection prompt can have widespread and unintended consequences across numerous interactions.

## Getting Started

### Prerequisites

- Python 3.x
- TensorFlow (>= 2.x)
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn
- NLTK

Installation
Clone the repository:

```bash
git clone https://github.com/SquashKiwi/prompt_injection_detection.git
cd prompt_injection_detection
```

(Optional) Create and activate a virtual environment:

```bash
python -m venv venv
source venv/bin/activate # On Linux/macOS
venv\Scripts\activate # On Windows
```

Install dependencies:

```bash
pip install tensorflow pandas numpy scikit-learn matplotlib seaborn nltk
```

## Evaluation

![corellation matrix](/assets/corellation_matrix.png)

## License

This project is licensed under the MIT License. See the LICENSE file for more details.

## Contributing

Contributions to this project are welcome! Please feel free to submit pull requests with bug fixes, new features, or improvements.
