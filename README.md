# Project 7: Stream Analysis - Amazon Reviews

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/AgatElite/stream-analysis/blob/main/Project_7_Stream_Analysis.ipynb)

## Overview

This project implements advanced **Stream Processing Algorithms** to analyze the Amazon Books Reviews dataset. Instead of loading the entire dataset into memory, the project treats data as a continuous stream, implementing the **Flajolet-Martin (FM) Algorithm** for estimating distinct elements (F0) and the **Alon-Matias-Szegedy (AMS) Algorithm** for estimating the second moment (F2).

The implementation focuses on memory efficiency and scalability, comparing algorithmic estimates against exact ground truth values calculated in real-time.

## Key Algorithms

* **Flajolet-Martin (FM):** Uses hash functions and trailing zero analysis to estimate the number of unique user IDs in the stream. Improved accuracy is achieved through a "median-of-averages" approach.
* **AMS Estimator:** Utilizes reservoir sampling and randomized variables to estimate the surprise requirement (second moment), identifying the frequency distribution of the data stream.

## How to Run

1. Click the **"Open in Colab"** badge above.
2. Run the first cell.
3. When prompted, upload your personal `kaggle.json` API token (downloadable from your Kaggle account settings). The notebook will automatically download the [Amazon Books Reviews](https://www.kaggle.com/datasets/mohamedbakhet/amazon-books-reviews) dataset and begin the stream processing.

## Repository Structure

* `Project_7_Stream_Analysis.ipynb`: The main notebook containing the stream simulation and algorithm implementations.
* `Stream_Analysis_Report.pdf`: The paper reporting the methods employed and the conclusions found in the project.
* `README.md`: Project documentation.
