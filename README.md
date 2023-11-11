
---

### Foxconn Industrial AI Data Challenge: Time Series Forecasting for Tool RUL Prediction

**Table of Contents:**
1. [Project Overview](#project-overview)
2. [Data](#data)
3. [Data Preprocessing](#data-preprocessing)
   - [Data Synchronization](#data-synchronization)
   - [Feature Engineering](#feature-engineering)
4. [Modeling](#modeling)
   - [Data Normalization](#data-normalization)
   - [Model Selection](#model-selection)
   - [Goal](#goal)
5. [Results](#results)
6. [Technologies Used](#technologies-used)
   
#### Project Overview:
The Foxconn Industrial AI Data Challenge centered on the crucial task of time series forecasting to predict the Remaining Useful Life (RUL) of industrial tools. Given the importance of proactive maintenance in industrial settings, accurately determining RUL can lead to optimal operational efficiency and reduced downtime. **Ranked 1st in my class for this challenge.**

<p align="center">
 <img src="https://github.com/tyrellto/RUL-tool-prediction/assets/61175343/8bc7fab3-ea52-433f-82ac-a475074f785d" width="600" alt="RUL Sample"/>
</p>

#### Data:
The dataset comprises vibration signal data for three different types of tools, inclusive of:
- PLC (Programmable Logic Controller) data
- Sensor data

#### Data Preprocessing:
1. **Data Synchronization**:
   - Sensor data was sampled to synchronize with the PLC data, ensuring that signals from different sources align temporally.

2. **Feature Engineering**:
   - Fourier signal filtering was applied to the vibration signal data to filter out noise and highlight significant frequency components.
   - Descriptive statistics such as mean, standard deviation, maximum, and skewness were computed for the vibration signals post-filtering.

#### Modeling:

1. **Data Normalization**: 
   - Before model training and testing, data was normalized to ensure that features have the same scale. This aids in faster convergence during model training and ensures that each feature contributes optimally to the predictive model.

2. **Model Selection**:
   - XGBoost, a gradient boosting algorithm, was chosen for its efficiency and capability to handle time series data effectively.

3. **Goal**:
   - The primary goal of the project was to predict the RUL of the tools. Given the features derived from the vibration signal data and other sources, the model provides an estimate of the time left before a tool requires maintenance or replacement.



#### Results:

In the context of the classroom setting, the model and methodology employed for this challenge proved to be exceptionally effective. The project was awarded the top score, culminating in an **A** grade. This distinction underscores the robustness and efficacy of the approach taken, positioning it as a potential benchmark for similar projects or challenges.

It's worth noting that the exact performance metrics or proximity to the optimal solution were not disclosed by the professor, possibly due to confidentiality or the proprietary nature of the challenge data and specifics. However, the top grade achieved is a testament to the model's superior performance relative to other solutions presented in the class.

---
