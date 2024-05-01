# 6600 Final Project

## Overview

This repo contains work by Corwin Dark for the final project in DSAN 6600. For my project, I chose to examine the utility of neural networks in improving the performance of statistical ensembles for financial time series prediction. I have store the most up to date version of my code in this folder.

## Files

-  dl_ens_exploration.ipynb

This file is meant to be run in the Google Colab cloud environment. It can be run on GPU or CPU, just comment out the calls to CUDA if the Colab instance does not have GPU access. This file contains all of the background code and plots used to create the report.

-  raw_data
This folder contains the zipped raw files of the financial time series data used for the paper. These datasets also contain the calculated prediction values from the statistical models. In an effort to speed up model compute time, we will move to pre-calculating all of the statistical model. Naming convention for this data is [ticker][year][increment][intervalval]_b[windowback]_f[predictionwindow]_[modelinitials]. Modelinitals = A-Arima, D-Dynamic Optimized Theta, C = Complex Exponential Smoothing, E = Auto Exponential Smoothing The order of model intials tells you order that data is stored in columns. Example: SPY2023min5_b10_f1_AC.
