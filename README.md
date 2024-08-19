## 전북대학교 원예학과 실험온실의 내부 환경 변수를 예측

### 목표

- 시계열 데이터를 이용한 머신러닝 딥러닝 기술을 적용 및 비교분석

- 시계열 딥러닝 모델인 LSTM을 간단한 레이어로 구성하여 날씨와 온실 미기후 자료를 활용하여 예측하는 모델을 만들어보자.

- Meta의 Prophet 모델을 테스트 해 보자.
  
- 대표적인 트리기반 머신러닝 모델인 RandoForest와 XGBoost를 stacking 하여 Ensemble 모델을 구축해보자.
  
- 더 나아가 이전 시간 온실 내부 환경 자료를 dummies로 활용해서 머신러닝 모델인 RandoForest와 XGBoost를 이용한 시계열 예측 모델을 만들어보자.
  
- 전체적으로 모델의 성능을 비교분석해보자.


<br>

### 데이터 셋

- 전북대학교 원예학과 실험 온실에서 수집한 온실 내부 데이터와 기상청 ASOS에서 수집한 외부 환경 데이터를 이용함.

- 수집한 데이터는 1시간 단위 데이터임.

- 2023년 5월 10일 부터 2024년 3월 19일 까지의 데이터로 학습하고, 2024년 3월 20일 부터 27일 까지의 데이터를 테스트 데이터로 사용하여 평가함.

- asos_download.py를 이용해서 기상청 ASOS 데이터를 다운받고, data_preprocessing.py에서 기상청 자료와 따로 수집한 온실 내부 환경 데이터를 전처리.

- data_EDA.ipynb에서 전체적인 데이터 구조를 시각화 하여 살펴봄.

- Microclimate_Modeling.ipynb에서 모델 학습 및 시각화.
