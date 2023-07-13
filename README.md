# Gitcoin Citizen Round Similarity Analysis

This repository contains the code and data for performing similarity analysis on the Gitcoin Citizen Round dataset. The analysis aims to identify and group similar addresses based on their voting and funding patterns.

## Table of Contents

- [Introduction](#introduction)
- [Getting Started](#getting-started)
- [Data](#data)
- [Similarity Analysis](#similarity-analysis)
- [Results](#results)

## Introduction

The Gitcoin Citizen Round is a dataset that captures the voting and funding activities of participants in the Gitcoin ecosystem. This similarity analysis focuses on identifying similar addresses based on their voting and funding patterns, allowing for the grouping of addresses with similar behavior.

## Getting Started

To run the similarity analysis, follow these steps:

1. Clone this repository to your local machine.
2. Install the required dependencies by running `pip install -r requirements.txt`.
3. Obtain the necessary API key from Optimismscan and update the `api_key` variable in the Jupyter Notebook (`similarity_analysis.ipynb`) with your API key.
4. Launch Jupyter Notebook by running `jupyter notebook` in the project directory.
5. Open the `similarity_analysis.ipynb` notebook.
6. Execute the cells in the notebook to perform the similarity analysis.

## Data

The dataset used for this analysis includes voting and funding information from the Gitcoin Citizen Round. It contains information such as addresses, voting counts, wallet age, funding counts, and transaction details.

## Similarity Analysis

The similarity analysis is based on cosine similarity, which measures the similarity between address features. The code calculates the cosine similarity matrix and groups together addresses with a similarity threshold above a specified value.

The analysis includes the following steps:

1. Data preprocessing: The data is prepared by encoding categorical features and selecting relevant columns for analysis.
2. Similarity matrix calculation: The cosine similarity matrix is computed based on selected features.
3. Similarity grouping: Addresses with similarity above a defined threshold are grouped together.
4. Compilation and uniqueness: Similar address groups are compiled while ensuring there are no duplicate rows within each group.

## Results

The analysis provides the following results:

- Cluster Grouping: Similar addresses are grouped together based on their voting and funding patterns. Each cluster represents a group of addresses with high similarity.


## Data
- [Dataset](https://huggingface.co/datasets/Poupou/Gitcoin-Citizen-Round)
- The other data was queried on the 12th of july

The results of the similarity analysis are printed to the console, displaying the cluster groups and their respective addresses.
