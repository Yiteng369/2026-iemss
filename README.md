# Explainable LSTM Forecasts for Hourly CO₂ Concentrations

[![Paper](https://img.shields.io/badge/Paper-PDF-blue)](./iemss2026_Yiteng.pdf)\
[![Dataset](https://img.shields.io/badge/Data-Zugspitze%20Station-green)](https://www.icos-cp.eu/)

## 📖 Introduction

This repository contains the official implementation of the paper:  
**"Explainable LSTM Forecasts for Hourly CO₂ Concentrations"** (iEMSs 2026).

Accurate short-term CO₂ forecasting is essential for monitoring background levels, detecting anomalous episodes, and supporting atmospheric modelling. While LSTM networks are effective at capturing nonlinear and multi-scale temporal dependencies in long time series, their use in environmental applications is often constrained by limited interpretability.

This work combines:

- **Engineered temporal features** (multi-scale lags, rolling means/variances, calendar indicators)  
- **Sequence-to-one LSTM forecasting model**  
- **Integrated Gradients attribution analysis** for feature-level interpretability  

The study shows that short-window rolling means and recent lagged CO₂ values dominate the model’s predictive behaviour, while seasonal indicators contribute moderately and variance-based features have limited influence.

---

## 🚀 Features

- Hourly CO₂ forecasting with a sequence-to-one LSTM  
- Integrated Gradients for global feature importance analysis  
- Long-term high-altitude CO₂ dataset (Zugspitze, 2002–2025)  
- Rich temporal feature engineering (3–168 hour lags and rolling windows)  
- Reproducible training and evaluation scripts

---

## 📚 Citation

If you use this code in your research, please cite:


@inproceedings{zhang2026explainable,
  title        = {Explainable LSTM Forecasts for Hourly CO2 Concentrations},
  author       = {Zhang, Yiteng and Pakrashi, Arjun and Dev, Soumyabrata},
  booktitle    = {International Environmental Modelling and Software Society (iEMSs)},
  year         = {2026}
}


------------------------------------------------------------------------

## Acknowledgements

-   CO₂ observations from the Zugspitze high-altitude monitoring station

-   Integrated Gradients method following Sundararajan et al. (2017)

-   LSTM-based time series forecasting inspired by recent work on atmospheric and air quality prediction
