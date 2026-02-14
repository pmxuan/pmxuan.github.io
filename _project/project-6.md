---
title: "Thesis Graduation"
# excerpt: "This thesis proposes the Beats-ODE model, which combines N-Beats and MTGODE to enhance traffic forecasting by learning temporal and spatial features through ODE. Additionally, the model integrates an explanation mechanism based on mask optimization, improving transparency and reliability.<br/><img src='/images/BeatsODE.png'>"
excerpt: |
    - **Purpose:** Traffic forecasting is the process of estimating traffic flow on routes and intersections in a transportation system. The goal
        of this prediction is to provide detailed and accurate information about traffic conditions, helping urban managers and drivers make
        smart decisions.
    - **Description:** Proposed a Traffic Forecasting Beats-ODE model with N-Beats blocks and MTGODE sublayers integrated into the
        model to improve traffic prediction. Stacked convolutional ODE blocks are used to learn temporal features, and graph convolutional
        ODE blocks are applied to learn spatial features. The use of ODE helps information flow from one layer to another continuously,
        increasing the accuracy of the model.
    - **Technologies:** Python, PyTorch, Scikit-learn, Numpy, Pandas, Folium, Matplotlib
collection: portfolio
---
# An Interpretable Model for Spatio-Temporal Traffic Forecasting
### Abstract:
Traffic forecasting is the process of estimating traffic flow on roads and intersections within a transportation system. The goal of this prediction is to provide detailed and accurate information about traffic conditions, helping urban management and drivers make informed decisions. In the past decade, traffic forecasting methods have rapidly evolved, especially with the expansion of artificial intelligence. Additionally, Explainable Artificial Intelligence (XAI) aims to address the challenge of making machine learning models more transparent and interpretable. In the context of traffic forecasting, model transparency is crucial for enhancing trust among the community and users. XAI in traffic prediction enables interpretability of the modeling and forecasting processes, helping users understand why a specific prediction is made.

Recognizing this issue, this thesis proposes a Beats-ODE model for traffic forecasting, integrating N-Beats blocks and the MTGODE submodule to improve predictive performance. In this model, stacked convolutional ODE blocks are employed to learn temporal features, while graph convolutional ODE blocks are used to capture spatial characteristics. The use of ODE allows continuous information flow between layers, enhancing model accuracy. Additionally, we integrate a traffic forecasting module with an explainability module based on mask optimization for regression tasks. This approach increases user trust in the model, as they can analyze key contributing factors and understand the reasoning behind specific predictions.

Furthermore, we conducted experiments to evaluate our model’s accuracy against state-of-the-art methods on two datasets: METR-LA and PEMS-BAY. The results demonstrate that our proposed approach outperforms existing baseline methods.

## Forecasting Architecture
<img src='/images/BeatsODE.png'>

## XAI Architecture
<img src='/images/Dynamask.png'>

## Dataset:
- I use the METR-LA and PEMS-BAY datasets, which can be downloaded and accessed from [Google Drive](https://drive.google.com/drive/folders/10FOTa6HXPqX8Pf5WRoRwcFnW9BrNZEIX).
- I follow the same data preprocessing steps as described in the study by the authors of the DCRNN paper [DCRNN](https://arxiv.org/pdf/1707.01926.pdf).

## Results:
- Traffic Forecasting
<img src="/images/METR.jpg"/>
<img src="/images/PEMS.jpg"/>
- XAI

<img src="/images/XAI.jpg"/>

**Repo:** [Github](https://github.com/pmxuan/GraduationThesis).