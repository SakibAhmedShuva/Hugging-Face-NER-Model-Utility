# Hugging Face NER Model Utility

A Python utility for loading and inspecting trained Named Entity Recognition (NER) models from Hugging Face. This tool provides quick access to model configuration details, including label schemas and entity mappings.

## Overview

This repository contains a Jupyter Notebook (`hf-ner-utility.ipynb`) that loads trained NER models from checkpoints and displays their configuration details. It supports various token classification models from the Hugging Face `transformers` library, including RoBERTa, DistilBERT, and other compatible architectures.

## Features

- **Model Agnostic**: Compatible with any Hugging Face token classification model using `AutoModelForTokenClassification`
- **Configuration Inspection**: Displays model architecture, label count, and label-to-ID mappings
- **Simple Integration**: Minimal setup required with straightforward usage
- **Error Handling**: Includes validation for model paths and loading operations

## Prerequisites

Ensure the following libraries are installed:

- PyTorch
- Transformers

Install dependencies via pip:

```bash
pip install torch transformers
```

## Usage

1. Clone or download the `hf-ner-utility.ipynb` notebook
2. Open the notebook in your preferred Jupyter environment (Jupyter Lab, Jupyter Notebook, or Google Colab)
3. Update the `model_load_path` variable with the path to your saved model checkpoint
4. Execute the cell to view the model's label configuration

## Sample Output

```
--- Model Label Information ---
Model type: distilbert
Total number of labels: 22

--- Label to ID Mapping ---
O: 0
B-Action: 1
B-ApplicationSpecific: 2
B-AuthenticationType: 3
B-IPAddress: 4
...
-----------------------------
```

## Contributing

Contributions are welcome! Please feel free to submit issues or pull requests for improvements and bug fixes.

## License

This project is open source and available under the MIT License.
