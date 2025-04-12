# COVID-19 Dynamics Modeling: SINDy, LSTM, Symbolic Regression, and AR(14)

## 📌 Overview
This repository explores COVID-19 epidemic dynamics using multiple modeling approaches:

- **Sparse Identification of Nonlinear Dynamical Systems (SINDy)**
- **Symbolic Regression**
- **Long Short-Term Memory (LSTM)** neural networks
- **Autoregressive (AR)** models (lag 14)

The goal is to identify interpretable governing equations and accurately forecast COVID-19 trends based on daily epidemiological data (Susceptible, Infected, Deaths, Recovered).

## 🚀 Objectives
- Perform data-driven modeling of COVID-19 dynamics (SIDR).
- Discover sparse, interpretable governing equations using SINDy and Symbolic Regression.
- Develop predictive models using LSTM and AR(14).
- Compare the performance of equation-based and neural network-based modeling.

## 🔧 Methodology

### 1. **Data Preprocessing**
- Extraction of daily cumulative COVID-19 cases and deaths.
- Computation of Susceptible (S), Infected (I), Deaths (D), Recovered (R) series.
- Normalization and smoothing (Savitzky–Golay filter).

### 2. **Sparse Identification (SINDy)**
- Polynomial feature library generation.
- Multi-task Lasso regression to derive sparse, interpretable equations for SIDR dynamics.
- Simulation of SIDR equations to validate against observed data.

### 3. **Symbolic Regression**
- Leveraged the PySR library for symbolic regression.
- Identified closed-form symbolic equations to describe SIDR dynamics without explicit derivative input.
- Analyzed complexity vs accuracy trade-offs.

### 4. **LSTM Neural Network**
- Trained LSTM on SIDR data from 2020–2021.
- Performed multi-step forecasting (3-month prediction).
- Evaluated accuracy through validation against observed epidemic curves.

### 5. **Autoregressive (AR) Model**
- Implemented an AR(14) model to predict future SIDR values using past 14-day observations.
- Benchmarked AR model predictions against LSTM and symbolic regression models.

## 📈 Results
- **SINDy and Symbolic Regression** successfully provided interpretable differential equations capturing epidemic trends.
- **LSTM and AR(14)** effectively forecasted short-term dynamics, with LSTM exhibiting superior accuracy for nonlinear patterns.
- Combination of analytical models (SINDy, SR) and predictive models (LSTM, AR) provided comprehensive insights into COVID-19 dynamics.

## ✨ Contributors
- George Habib
- Roni Bou Saab 