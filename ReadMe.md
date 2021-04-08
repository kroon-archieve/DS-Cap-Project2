# Capstone Project 2 [김가연, 이동훈]

## 재고 관리를 위한 단기(6개월) 수요 예측 모델 생성

## 개요

  본 프로젝트는 회사가 재고를 최적화하고 판매를 극대화할 수 있도록 수요 예측 모델을 생성하는 것을 목표로 힌디. 모델에서 사용하는 학습 데이터셋의 기간 조절, 모델 구조 변경을 통해 성능이 가장 좋은 단기(6개월) 수요 예측 모델을 생성하고자 하였다.

---
## 사용한 데이터 셋
Forecasts for Product Demand: Make Accurate Forecasts for Thousands of Different Products
- FelixZhao, Kaggle,https://www.kaggle.com/felixzhao/productdemandforecasting
-  License: GPL 2

---
## 생성한 모델
- Baseline:  ARIMA 
- 비교대상: XGBoost, LSTM
- LSTM 모델 구조

![lstm_](https://user-images.githubusercontent.com/70473564/113970703-49fdde00-9872-11eb-8808-a7c3a6a310d6.png)



---
## 결과

|               | MAE | RMSE |
|:-----------:|:------:|----------:|
|ARIMA    |1,566,273.08 | 2,035,642.05|
|XGBoost |669,591.5    | 999,821.2|
|LSTM      |842,659.64|1,148,008.08 |

---
## 참고문헌

- Bandara, Kasun, et al. “Sales Demand Forecast in E-Commerce Using aLong Short-Term Memory Neural NetworkMethodology.” Faculty of Information Technology, Monash University, Melbourne, Australia, Springer, 2021.
- Gołąbek, Marta, et al. “Demand Forecasting Using Long Short-TermMemory Neural Networks.” Karlsruhe University of Applied Sciences, 2020.
---
## 참고자료
- Brownlee, Jason. “How to Create an ARIMA Model for Time Series Forecasting in Python.” Machine Learning Mastery, 9 Dec. 2020, machinelearningmastery.com/arima-for-time-series-forecasting-with-python/.
- Brownlee, Jason. “How to Develop LSTM Models for Time Series Forecasting.” Machine Learning Mastery, 27 Aug. 2020, machinelearningmastery.com/how-to-develop-lstm-models-for-time-series-forecasting/.
- Brownlee, Jason. “How to Use XGBoost for Time Series Forecasting.” Machine Learning Mastery, 18 Mar. 2021, machinelearningmastery.com/xgboost-for-time-series-forecasting/.



