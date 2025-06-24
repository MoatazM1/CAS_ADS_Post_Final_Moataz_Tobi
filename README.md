# 📦 CAS ADS Final Project — Swiss Post Package Sorting Optimization

This repository contains the final CAS Advanced Data Science (ADS) project submitted by **Moataz & Tobi**. The project addresses real-world performance challenges in **Swiss Post's package sorting centers**, using predictive and prescriptive modeling techniques.

---

## 🚀 Objective

To detect and prevent **performance degradation** caused by overloaded chutes, by developing and comparing multiple machine learning strategies:

1. 🎯 Predicting delays using time series data
2. 🔄 Rerouting ZIP codes dynamically to optimize chute assignments using Reinforcement Learning
3. 📉 Reducing processing time through smart intervention strategies

---

## 🧠 Project Structure

| File | Description |
|------|-------------|
| `1Random_forest.ipynb` | Baseline model using tree-based methods |
| `2LSTM.ipynb` | Time series delay prediction using LSTM |
| `3Reinforcement_Learning.ipynb` | Early RL attempt for dynamic decision-making |
| `3Reinforcement_Learning_With_Issues.ipynb` | Cleaned version using real performance data |
| `POST_SORTING_CAS-ADS-Project.docx` | 📄 Final report including problem, methods, evaluation |
| `data4day.csv` | 4-day ZIP + chute + hour dataset |
| `data4day_with_issues.csv` | Augmented with high-load edge cases for training/testing |

---

## 🧪 Key Methods

- 📊 Exploratory Data Analysis
- 🌲 Random Forest Regressors
- 📈 LSTM Time Series Forecasting
- 🤖 Reinforcement Learning with Stable-Baselines3
- 🧪 Simulated environment using `gymnasium` and custom `PackagingCenterEnv`

---

## 📉 Sample Metrics

- Overload detection accuracy
- Processing time before vs. after optimization
- Agent reward progression over episodes
- Visualization of system delays, queues, and actions taken

---

## 📎 Results Summary

- Tree models were interpretable but missed edge overloads
- LSTM captured patterns but lacked responsiveness
- RL agent **actively reduced overload and delay** by rerouting intelligently
- Generated dashboards and performance heatmaps

---

## 📦 Dataset

- Hourly package counts and average processing time
- Chute ID, ZIP code, scanning station
- Includes real and artificially injected congestion scenarios

---

## 🛠 Dependencies

```bash
pip install gymnasium stable-baselines3 matplotlib seaborn pandas numpy
