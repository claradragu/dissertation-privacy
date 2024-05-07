# Dissertation Notebook

## Overview
This Jupyter notebook contains a comprehensive analysis of the impact of differential privacy mechanisms on synthetic datasets. The project demonstrates how differential privacy methods affect the utility of data and provides insights through various analytical techniques such as clustering and regression.

## Table of Contents
1. [Setup](#setup)
2. [Data Generation](#data-generation)
3. [Noise Application Mechanisms](#noise-application-mechanisms)
4. [Augmenting Data with Noise](#augmenting-data-with-noise)
5. [Visualization of Results](#visualization-of-results)
6. [Statistical Analysis](#statistical-analysis)
7. [Anonymeter Evaluation](#anonymeter-evaluation)
8. [Linkability Evaluation](#linkability-evaluation)
9. [Inference Evaluation](#inference-evaluation)

## Setup
1. **Import Libraries**  
   The notebook begins by importing all the necessary Python libraries required for data manipulation, machine learning, visualization, and privacy protection.

2. **Generate Data**  
   The `generate_data(size)` function creates synthetic data using the Faker library to simulate individuals with attributes like name, age, email, salary, etc.

## Noise Application Mechanisms
- **Laplace Mechanism**  
  The `apply_laplace_mechanism` function applies Laplace-distributed noise to a dataset.

- **Gaussian Mechanism**  
  The `apply_gaussian_mechanism` function adds Gaussian noise to a dataset to ensure (epsilon, delta)-differential privacy.

## Augmenting Data with Noise
- The `apply_noise_mechanisms` function applies both Laplace and Gaussian mechanisms to the synthetic dataset.

## Visualization of Results
- The `plot_comparisons` function visualizes original vs. noised salary distributions across different privacy levels.

## Statistical Analysis
- **Metrics Calculation**  
  The `compute_statistics` function calculates various metrics (mean, median, standard deviation, etc.) between the original and noised datasets.

- **Comparative Analysis**  
  Functions like `analyze_noised_salaries` and `enhance_statistics_with_original` provide comparative analyses between original and noised datasets.

## Anonymeter Evaluation
- **Privacy Risk**  
  Functions like `SinglingOutEvaluator` evaluate the risk of identifying an individual based on synthetic data.

## Linkability Evaluation
- **Auxiliary Columns**  
  The `LinkabilityEvaluator` analyzes the ability to re-identify individuals using auxiliary attributes.

## Inference Evaluation
- **Attribute Prediction**  
  The `InferenceEvaluator` assesses the ability to predict specific attributes using auxiliary data.

## Notes
- Adjust the input parameters, dataset sizes, and visualization parameters as needed to analyze different privacy configurations.
- Ensure that the appropriate libraries are installed before running the notebook.

