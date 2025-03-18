# Ethics, Fairness, and Explanation in AI - Spring 2025

This project is part of the course **"Ethics, Fairness, and Explanation in AI"** at **Imperial College London** for the Spring term 2025. The assignment explores and evaluates feature attribution and counterfactual explanations in machine learning models. The project is divided into three main tasks: Exploratory Data Analysis, Feature Attribution Explanations, and Counterfactual Explanations.

## Table of Contents
- [Overview](#overview)
- [Project Structure](#project-structure)
  - [1. Exploratory Data Analysis](#1-exploratory-data-analysis)
  - [2. Feature Attribution Explanations](#2-feature-attribution-explanations)
  - [3. Counterfactual Explanations](#3-counterfactual-explanations)
- [Requirements](#requirements)
- [Usage](#usage)
- [Results](#results)
- [References](#references)

## Overview

This project focuses on understanding and evaluating various techniques for explaining machine learning models. The assignment is divided into three key parts:

1. **Exploratory Data Analysis**: Analyzing the Titanic dataset to identify patterns and trends, predicting important features for a neural network, and suggesting additional methods for exploration.
2. **Feature Attribution Explanations**: Implementing the SHAP method and comparing it with other attribution methods (Shapley Value Sampling and DeepLIFT) using the Captum library.
3. **Counterfactual Explanations**: Designing and implementing a distance metric for counterfactual explanations, and comparing two methods for generating counterfactuals: Nearest-Neighbour Counterfactual Explainer (NNCE) and the Wachter et al. (WAC) method.

The project includes implementation code and a report that summarizes key results, observations, and conclusions.

## Project Structure

### 1. Exploratory Data Analysis

The task involves:
- Analyzing the **Titanic dataset** to identify patterns and trends.
- Predicting which features are most and least important for a neural network.
- Suggesting additional exploratory analysis methods to better understand the data.

Key results and insights are provided in the `titanic_analysis.ipynb` notebook.

### 2. Feature Attribution Explanations

The task involves implementing the following methods and comparing their performance:
- **SHAP**: Implemented in `shap_explanation.py`.
- **Shapley Value Sampling**: Implemented in `shapley_value_sampling.py`.
- **DeepLIFT**: Implemented in `deeplift_explanation.py`.

We evaluate these methods on both the Titanic and Dry Bean datasets, comparing their **infidelity** and **computational efficiency**.

Results and comparisons are provided in the `evaluation_results/` folder.

### 3. Counterfactual Explanations

This task focuses on designing and implementing counterfactual explanations using two methods:
- **Nearest-Neighbour Counterfactual Explainer (NNCE)**: Implemented in `nnce.py`.
- **Wachter et al. (WAC)**: Implemented in `wac.py`.

Additionally, we design a **distance metric** for generating counterfactual explanations, implemented in `distance_metric.py`. We evaluate the generated counterfactuals using metrics like **proximity**, **validity**, and **plausibility**.

You can install the dependencies using:

```bash
pip install -r requirements.txt
```

## Usage

- To run the exploratory data analysis, open `titanic_analysis.ipynb` and execute the cells.
- For feature attribution and counterfactual explanation tasks, run the Python scripts in the corresponding directories.
- Evaluate the results by reviewing the generated plots and results in the `evaluation_results/` and `counterfactual_results/` directories.

## Results

The report summarizes the results of each task, including key observations and conclusions. The full report can be found in `report.pdf`.

## References

- **SHAP**: [https://github.com/slundberg/shap](https://github.com/slundberg/shap)
- **Captum**: [https://captum.ai/](https://captum.ai/)
- **Wachter et al. (WAC)**: Wachter, S., Mittelstadt, B., & Russell, C. (2017). *Counterfactual Explanations without Opening the Black Box: Automated Decisions and the GDPR*. Proceedings of the 2017 CHI Conference on Human Factors in Computing Systems.
