# EY Water Quality Prediction (R²: 0.82)

## Overview

This repository contains my solution for the EY Data Challenge, where the objective was to predict water quality using satellite (Landsat) and climate (TerraClimate) datasets. The evaluation metric was the average R² score, making this a performance-focused, leaderboard-driven problem.

## Problem Approach

The main challenge was not just building a model, but effectively combining multiple datasets and improving prediction accuracy under competition constraints.

I approached the problem in stages:

* **Data Understanding & Integration**
  The data came from different sources with varying structures. The first step was to align and merge Landsat and TerraClimate features correctly so that each observation had consistent inputs.

* **Handling Missing Values & Noise**
  The dataset contained missing and inconsistent values. Instead of complex imputation, I focused on practical cleaning techniques that preserved useful signals without overcomplicating the pipeline.

* **Feature Selection**
  Not all features contributed equally to the model. I experimented with subsets of features and removed less useful ones to reduce noise and improve stability.

* **Model Building & Iteration**
  Multiple models and configurations were tested. The focus was on iterative improvement — adjusting parameters, testing performance, and refining the approach based on results rather than sticking to a single method.

## Key Findings

* Combining **satellite + climate data** significantly improved predictive performance compared to using a single source.
* Simpler preprocessing worked better than overly complex transformations for this dataset.
* Model performance improved gradually through tuning rather than a single major change.
* Consistent feature alignment across datasets was critical for achieving stable results.

## Result

After multiple iterations and refinements, the final model achieved:

**Average R² Score: 0.82**

This reflects the model’s ability to generalize well on unseen data and perform competitively on the leaderboard.

## Dataset

The dataset used in this project is part of the EY Challenge and is not included in this repository due to confidentiality.

To run this notebook:

* Place the datasets inside a `data/` folder
* Ensure file names match those referenced in the notebook

## Repository Structure

* `EY-FINAL-CHECK.ipynb` → Complete implementation
* `output_preview.pdf` → Executed notebook outputs and results
* `screenshots/` → Key outputs for quick viewing

## Note

Since the dataset is not publicly available, the notebook will not run as-is. The PDF and screenshots provide a full view of the execution and results.

## Takeaway

This project highlights my ability to work on a competitive ML problem, iterate quickly, and improve model performance through structured experimentation.
