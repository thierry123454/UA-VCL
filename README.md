# UDL Mini-Project: Continual Learning with VCL and UA-VCL on Permuted MNIST

This repository contains code for a mini-project on extending Variational Continual Learning (VCL) to get Uncertainty-Aware VCL (UA-VCL). The project compares several approaches—including standard VCL (with and without coresets), UA-VCL, and Elastic Weight Consolidation (EWC)—and provides experiments for both classification and regression tasks on the Permuted MNIST dataset.

## Overview

- **Continual Learning Methods:**  
  - **VCL:** Uses Bayesian inference with a Gaussian mean-field approximation.
  - **UA-VCL:** Extends VCL by incorporating uncertainty-aware coreset selection and KL regularization.
  - **EWC:** Regularizes parameter updates using the Fisher Information Matrix.

- **Experiments:**  
  Models are trained sequentially on permuted versions of MNIST. Results include average test accuracy, RMSE, and accuracy curves across tasks. Hyperparameters such as coreset size, EWC lambda, and the UA-VCL hyperparameter $\alpha$ are varied to study their impact.

- **Visualizations:**  
  Plots are generated to illustrate:
  - Average test accuracy over tasks.
  - The impact of different coreset sizes.
  - Average test RMSE over tasks.
  - Visualizations to study the effect of uncertainty-aware KL regularization and \(\alpha\) on performance.
