# Automated Fact-Checking in Polish

This repository contains the datasets, code, and resources used in the Master's thesis titled "Translating Check-worthiness: Adapting Advanced Claim Detection Models for Automated Fact-Checking to a Low-Resource Language," authored by Aleksy Gałkowski, under the supervision of Yevgeniy Golovchenko and Jeppe Søndergaard Johansen at the University of Copenhagen.

## Overview

The thesis focuses on adapting cutting-edge BERT-based classification methods to enhance claim detection for check-worthy claims in the Polish language. This involves a comparative study of machine-translated versus Polish-sourced data for training check-worthiness detection models in Polish political statements.

## Repository Structure

- `data/`: This folder contains raw data files and metadata associated with the datasets used in the thesis.
- `Codebook_FactRank_EN.pdf`: The coding manual adapted from FactRank, providing guidelines for annotating claims as factually relevant, non-relevant, or non-factual.
- `demagog-scrape.ipynb`: Jupyter notebook used to scrape and preprocess data from Demagog.org.
- `model-training.ipynb`: Notebook containing the scripts for training and evaluating the classification models.
- `translation.ipynb`: Notebook used for translating English datasets to Polish using Google and DeepL APIs.

## Data Description

Data used in this study comes from several sources:
- **OPL (Originally Polish dataset)**: Collected from Demagog.org and other related texts.
- **CT24 (CheckThat! 2024 dataset)**: Used for check-worthiness prediction, originally in English and translated to Polish (GMT - with Google, and DMT - with DeepL) for this study.

## Usage

To run the notebooks, you will need Python 3.x and the following libraries:
- `pandas`
- `numpy`
- `scikit-learn`
- `transformers`
- `spaCy`
- `selenium`
- `requests`

Or install the necessary libraries from requirements.txt using pip:

```bash
pip install -r requirements.txt
