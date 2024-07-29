
# Poetry Generation with GPT-2

Welcome to the Poetry Generation with GPT-2 project! This project focuses on generating poetry using the GPT-2 model.

## Introduction

Poetry generation involves creating poetic text based on the context provided. In this project, we leverage the power of GPT-2 to generate poetry using a dataset of poems.

## Dataset

For this project, we will use a custom dataset of poems. You can create your own dataset and place it in the `data/poems.csv` file.

## Project Overview

### Prerequisites

- Python 3.6 or higher
- PyTorch
- Hugging Face Transformers
- Datasets

### Installation

To set up the project, follow these steps:

```bash
# Clone this repository and navigate to the project directory:
git clone https://github.com/your-username/gpt2_poetry_generation.git
cd gpt2_poetry_generation

# Install the required packages:
pip install -r requirements.txt

# Ensure your data includes poems. Place these files in the data/ directory.
# The data should be in a CSV file with one column: poem.

# To fine-tune the GPT-2 model for poetry generation, run the following command:
python scripts/train.py --data_path data/poems.csv

# To evaluate the performance of the fine-tuned model, run:
python scripts/evaluate.py --model_path models/ --data_path data/poems.csv
