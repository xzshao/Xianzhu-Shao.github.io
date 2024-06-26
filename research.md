---
layout: page
permalink: /research/index.html
title: research
---

*I appreciate your interest in my research so far and look forward to doing more valuable research with you in the future!!*

## Introduction


## Research Projects
### ISFormer:IMPROVED SEASONAL TRANSFORMER FOR POWER LOAD FORECASTING [First Author]
**Abstract:** There is an urgent need for intelligent systems to drive the development of global power systems. We
propose a high-precision and high-efficiency time-series prediction model, ISFormer, for short-term
high-granularity prediction of power systems based on the state-of-the-art Transformer architecture.
Previous models are based on the auto-correlation sequence-attention mechanism, however, is inef-
ficient and heavily reliant on the sample size at the sequence level. In this paper, we incorporate
the highly efficient distillation-attention mechanism and the time-sequence decomposition module
as our Transformer model kernel. The Time2Vec module is employed as the temporal information
embedding module of the model, which enhances the predictive performance and seasonal capture
ability of the model. The predictive efficacy of four distinct prediction granularities was evaluated
on four public datasets. On average, ISFormer exhibited a reduction in MSE and MAE of over 10%
compared to the existing SOTA model. The efficacy and significance of each module proposed in
this paper were assessed through comprehensive ablation experiments. In terms of time efficiency,
ISFormer demonstrated a reduction in MSE and MAE of over 30% compared to the SOTA model in
each prediction task.
<br>**Keywords:** Transformer · Power Forecasting · Autoformer · Time2Vec · Distillation Attention Mechanism
<img src="/images/Table_ISFormer_result.png" > 
<img src="/images/Fig_ISFormer_resut2.png" > 
<img src="/images/Fig_ISFormer_resut.png" > 


### A Dynamic Cost-Adjusted Adacost Model for Credit Scoring of Smallholder Farmers[First Author]
**Abstract:**  Credit scoring models have been constrained by the problem of data imbalance. In this paper, we propos
e a dynamic cost-adjusted Adacost credit scoring model to improve its prediction accuracy. This model enriches th
e existing research methods on credit problems of smallholder farmers and opens up new avenues for the establish
ment of credit scoring models for smallholder farmers. This paper has three research highlights. Firstly, by introdu
cing a variable cost-sensitive function, each sub-model generated by the Adacost model adapts to the changing mis
classification costs. As a result, the sample weights and model weights in the subsequent sub-models that are assoc
iated with the previous ones are dynamically adjustable. This overcomes the weakness of the traditional Adacost m
odel that ignores the dynamic impact of cost-sensitive functions on sample weights and model weights. Secondly, 
by introducing PCA and using the principal components after dimension reduction for modeling, the redundancy o
f data features is removed. Thirdly, we propose an exponential cost loss function that combines the exponential fun
ction and the variable cost-sensitive function. This causes the misclassification cost of default samples between adj
acent sub-models to increase exponentially, thereby improving the efficiency of model training. Using the data of a
gricultural loans from a commercial bank in China as empirical data and comparing with seven baseline models in
cluding Adaboost, Adacost, Cost RF, Cost XGBoost, Cost SVM, Cost GBDT, and Cost DT, we found that the prop
osed dynamic cost-adjusted Adacost model outperformed the other models. Robustness tests were conducted using
two publicly available loan datasets from UCI, and the results showed that the dynamic cost-adjusted Adacost mo
del performed better than the Adaboost and Adacost models.
**Keywords:** Data imbalance, Adacost, Cost-sensitive, Credit prediction
<img src="/images/p1.png" > 

### Time Series Prediction: Machine Learning Models Based on Rolling-ICEEMDAN Methods[Fourth Author]
The usual EMD,EEMD,ICEEMDAN etc. methods of prediction after temporal decomposition (One-Dimensional->Higher-Dimensional) are almost always wrong because of serious data leakage problems, so the predictions obtained are very good. My research group and I proposed **Rolling-ICEEMDAN Methods**, which is an adaptive **decomposition-prediction-fusion** scheme that solves the data leakage problem well and also shows good performance.
<img src="/images/p2.png" > 

## Work Projects

### SOH Prediction for Lithium Batteries: Highly Precise Long-Term Prediction Models based on Transformer Architecture
Time series forecasting using deep learning methods is often based on the seq2seq method, which does not allow true sense of the long-term time series forecasting in the word. The field of lithium battery SOH long-term prediction in previous research articles has chosen to fit empirical formulas and use the obtained empirical formulas to perform long-term prediction. I independently developed a forecasting model based on the transformer architecture, which requires only a small number of samples to realize a high-precision long-term forecasting model, carried out a lot of work to improve this model, so that the model can realize the long-term forecasting under different working conditions. The model has now become the core algorithm of more mature core design software in the industry.
<img src="/images/Fig_LongTerm_result.png" > 
<img src="/images/Fig_LongTerm_25_75.png" > 

### SOH Prediction for BMS System
Battery Management System (BMS) is a very important part of new energy vehicles. The state of health (SOH) of Li-ion batteries is difficult to measure in this process, and it is necessary to measure the SOH by current, voltage, and other characteristics.I independently developed a real-time prediction model of Li-ion battery degradation life based on a deep learning framework, which predicts battery life degradation at a certain period of time in the future just by using the dq/dv curves and the capacity-voltage curves. Under 140 test conditions (different charging policies), the maximum error of the model is within 1%.
<img src="/images/Fig_BMS_CV_curve.png" > 
<img src="/images/Fig_BMS_TRI_result1.png" > 
<img src="/images/Fig_BMS_pred_result.png" > 

### SOH Prediction for Lithium Batteries: An Improved Deep Learning model Based on Seq2Seq
SOH prediction of lithium batteries is a very hot topic in recent years, and has an important position in the BMS system, but 90% of the existing research is to predict only one point in the future through historical data, and the error is higher, I have been working on the algorithm development for about two months for this problem, and finally constructed a high-performance SOH prediction model, which can predict 80% of the future SOH changes by inputting 20% of the data, and can also flexibly input n SOH data points to predict the future m SOH data points(*the prediction accuracy is shown in the CV or Publication*).
<img src="/images/SOH_LSTM2.png" > 


### Solid-state Diffusion Coefficient Correction for Lithium Batteries: a High-Performance Parallel Simulated Annealing Algorithm
Simulated annealing algorithm (SA) has a strong global optimization ability, but SA is serialized algorithm, it cannot converge quickly in a short time on engineering problems with long single-step computation time, it is easy to fall into the local optimum, I greatly improve the optimization ability of SA by adding the techniques of **rewarming**, **adaptive annealing**, **randomly selecting the sampler**, **Lévy flight sampling**, and **exponentially distributing the samples** in simulated annealing algorithm, and I finally **parallelize** SA.

<img src="/images/HIGH_SA.png" > 

### Exploration of High-Performance Large Sparse Matrix Solvers
Solving large sparse matrices is a performance bottleneck often encountered in the field of computational fluid dynamics (of course, it is also very common in the field of AI Algorithm). For example, COMSOL uses pardiso is a high-performance sparse matrix solver, the direct solver has a very high accuracy, but often in the process of large sparse matrices is very slow or can not be calculated, the iterative solver is to lose accuracy through the loss of make large sparse matrices to be solved.
I spent about a month exploring almost all high-performance solver frameworks, and also accumulated more development experience, including ***PARDISO, CUPY, JAX, TAICHI, PETSc, AMGX***, etc.. Finally, I improved the computational performance of a process algorithm by nearly two orders of magnitude.

---
*Due to some technical terms, I can't provide project details for the last three projects, so if you're interested, please contact me at my email and maybe we can set up a meeting to talk about it together!*
<br>

---
**END**
