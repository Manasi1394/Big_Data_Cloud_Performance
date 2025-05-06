
# Energy Utilization and Optimization Using Analytics and Machine Learning

> **In Brief:**  
> Rising cloud workloads are inflating power use and carbon emissions.  
> Analyzed energy metrics from a simulated environment and applied ML to forecast demand.  
> Models suggest a potential 15–20% efficiency gain with smarter workload allocation.

## Table of Contents
1. [Background and Overview](#background-and-overview)  
2. [Data Structure Overview](#data-structure-overview)  
3. [Executive Summary](#executive-summary)  
4. [Insights Deep Dive](#insights-deep-dive)  
5. [Recommendations](#recommendations)

---

## Background and Overview
Data analytics and machine learning techniques are applied to improve energy efficiency in cloud computing environments. The approach involves:

- Using **descriptive analytics** to examine historical system performance.  
- Applying **predictive models** to anticipate future resource demands.  
- Leveraging **prescriptive methods** to optimize resource usage and reduce waste.

Machine learning helps identify patterns in workloads, enabling more efficient energy use without compromising performance. Rising demand for cloud services has increased data center energy consumption, leading to higher electricity costs and greater carbon emissions. Performance and energy metrics from a simulated cloud environment are analyzed to explore optimization opportunities and reduce environmental impact. Key challenges include reactive management, inefficient resource utilization, and high operational costs.

---

## Data Structure Overview
![Cloud Workload Metrics Overview](https://github.com/user-attachments/assets/c1a1a48e-77e2-4988-8688-c73dc9b61ad2)  

![image](https://github.com/user-attachments/assets/317897df-e1fc-4fba-b4bd-63ad333e3b71)

Collected metrics include CPU and memory usage, power consumption, network traffic, and execution time for tasks, along with **derived metrics** such as ***Energy Efficiency Ratio (EER)** and **Sustainability Index (SI)***.

---

## Executive Summary
In 2024, global energy consumption rose by 2.2%, with cloud computing contributing significantly due to data center expansion and increased digital demand. Carbon dioxide concentrations reached 420 ppm in 2023—a 10% rise over the past 20 years. Energy-aware system optimization is critical to reducing both power usage and emissions.

Analysis of simulated cloud workloads identified inefficiencies across usage clusters. By applying predictive modeling and optimization techniques, a potential 15–20% reduction in power consumption and associated emissions was observed.

To enable real‑time decision‑making, the proposal is to track EER and SI as operational metrics, establish threshold‑based alerts, and build dashboard visualizations so that teams can automatically trigger scaling or workload redistribution when efficiency degrades.

#### Power and Emissions
![Power vs CO₂ Emissions](https://github.com/user-attachments/assets/12753044-338d-4808-9f16-d5e0f68784b3)  
*Power consumption and CO₂ emissions move in lockstep, underscoring the direct environmental cost of energy use.*

#### Workload Clustering
![Workload Consumption Clusters](https://github.com/user-attachments/assets/377062a2-bf20-4ad8-93a2-2210be11e197)  
*Clusters showing High, Moderate, and Low consumption workloads.*

---

## Insights Deep Dive

### Correlation Analysis
![Correlation of SI and EER with System Metrics](https://github.com/user-attachments/assets/71a5cbd0-7642-409a-9602-ae5806119b10)  
*Correlation analysis shows that sustainability metrics like SI and EER are weakly correlated with individual metrics such as CPU or memory usage. Broader system behavior plays a greater role in energy performance than any single metric.*

### Improving Efficiency Strategies
Efficiency gains are achieved through smarter task scheduling, hardware configuration tuning, and load balancing improvements.

![Efficiency Strategies Impact](https://github.com/user-attachments/assets/831e7a32-13d3-4501-8eaf-5d4e235bfdcb)  
*Implementing energy‑efficient strategies leads to measurable declines in power use.*

### Metric‑Based Insights
![Metric-Based Energy Insights](https://github.com/user-attachments/assets/28986f79-3b8d-4084-ba13-460459b43b83)  
*Higher Sustainability Index and Efficiency Ratios align with lower power usage, validating these metrics as practical levers for optimization.* 

Tracking EER (watts per instruction) and SI (grams CO₂ per second) over time quantifies the impact of optimization.

### Forecasting Power Consumption
```python
from statsmodels.tsa.seasonal import seasonal_decompose

# Decompose the power consumption series to reveal trends and seasonality
decomposition = seasonal_decompose(data["Power_Consumption"], model="additive")

# Predict future power needs using a regression model trained on historical consumption and workload features
forecast = linear_regression_model.predict(future_dates)
```

Several predictive models (Linear Regression, Random Forest, XGBoost, LSTM) were evaluated using MAE and RMSE.

![Forecasting Model Comparison](https://github.com/user-attachments/assets/38c45e73-eef4-4624-95f1-7bcb614dabb9)  
*Forecasted consumption that can lead to effiecient energy resource planning and management.*

---

## Recommendations
1. **Adopt Renewable Energy**: Invest in solar, wind, or hydropower to offset carbon emissions.  
2. **Implement Energy Efficiency Measures**: Optimize operational processes and upgrade to energy‑efficient hardware.  
3. **Predictive Autoscaling**: Integrate forecasting models into autoscaling policies to smooth demand peaks.  
4. **Continuous Monitoring**: Build dashboards tracking EER and SI, with alerts for anomalous spikes.  
5. **Stakeholder Education**: Share insights and best practices to foster organizational commitment to sustainability.
