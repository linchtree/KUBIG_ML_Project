**1. EDA / Data Wrangling**
 - 결측치 탐지 및 제거 or 보간 (필수)
 - 중복데이터 탐지
 - Outlier 탐지 (탐지 후 제거할지 아닐지 판단과 그 근거)
 - 자료의 표준화 or 정규화 (필수는 아니며 만약 표준화 혹은 정규화를 할 경우 근거)
 - 불균형 자료일 경우 보완 (SMOTE)
 - 범주형 자료 Encoding
 - 데이터 시각화를 통해 인사이트 혹은 의문점 얻기 / 필요 없어 보이는 변수 제거 가능
 - 특성 변수 선택 (SelectKBest / SelectFromModel)
 - 파생변수 </br></br></br>


**2. 특성변수의 차원 축소 / 모형의 정밀화를 위해 군집분석 (안 해도 상관 x)**
 - PCA, t-SNE 등등 (차원 축소)
 - K-means Clustering (군집화) : 군집을 만든 뒤에 군집 별로 모형 분석 </br></br></br>


**3. 분류를 위한 모형 탐색**
- 로지스틱 회귀 / LDA / Random Forest (Bagging) / XGBoost / LightGBM / CatBoost 등등
- Validation Set 이용하여 Hyperparameter 튜닝
- (1) 모형의 성능 비교 (예측의 측면)
- (2) 특성변수의 중요도와 특성변수의 목적변수에 대한 기여도 (해석의 측면) </br></br></br>
