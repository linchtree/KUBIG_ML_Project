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



----------------------------------------------------------------------------------------
**Feature 설명**

* index

* gender: 성별

* car: 차량 소유 여부

* reality: 부동산 소유 여부

* child_num: 자녀 수

* income_total: 연간 소득

* income_type: 소득 분류
    * ['Commercial associate', 'Working', 'State servant', 'Pensioner', 'Student']

* edu_type: 교육 수준 
    * ['Higher education' ,'Secondary / secondary special', 'Incomplete higher', 'Lower secondary', 'Academic degree']

* family_type: 결혼 여부
    * ['Married', 'Civil marriage', 'Separated', 'Single / not married', 'Widow']

* house_type: 생활 방식
    * ['Municipal apartment', 'House / apartment', 'With parents', 'Co-op apartment', 'Rented apartment', 'Office apartment']

* DAYS_BIRTH: 출생일
    * 데이터 수집 당시 (0)부터 역으로 셈, 즉, -1은 데이터 수집일 하루 전에 태어났음을 의미

* DAYS_EMPLOYED: 업무 시작일
    * 데이터 수집 당시 (0)부터 역으로 셈, 즉, -1은 데이터 수집일 하루 전부터 일을 시작함을 의미 (양수 값은 고용되지 않은 상태를 의미함)

* FLAG_MOBIL: 핸드폰 소유 여부

* work_phone: 업무용 전화 소유 여부

* phone: 전화 소유 여부

* email: 이메일 소유 여부

* occyp_type: 직업 유형													

* family_size: 가족 규모

* begin_month: 신용카드 발급 월
    * 데이터 수집 당시 (0)부터 역으로 셈, 즉, -1은 데이터 수집일 한 달 전에 신용카드를 발급함을 의미

* credit: 사용자의 신용카드 대금 연체를 기준으로 한 신용도 **(Target Variable)**
    * => 낮을 수록 높은 신용의 신용카드 사용자를 의미함
