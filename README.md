# Data-Analysis

혼자 해보는 Data 분석 개인 프로젝트 여러개 업로드 예정

1. 자동차 판매 예측 프로젝트


# 🚗 고객 특성 기반 자동차 급 추천 프로젝트

## 🏁 프로젝트 목표
- 고객의 특성(성별, 재산, 소득 등)을 기반으로  
- 구매 가능한 자동차의 **급(class)** 을 예측한다.
- 고객에게 "이 고객님께 어울리는 자동차 급은 이 정도입니다!" 하고 추천하는 것을 목표로 한다.

---

## 🛠 사용한 기술 스택
- Python
- Pandas, NumPy (데이터 처리)
- Matplotlib, Seaborn (데이터 시각화)
- Scikit-learn (머신러닝 분류 모델)
- (필요시) XGBoost

---

## 📦 데이터 설명
- 주요 컬럼:
  - `성별`
  - `연 소득`
  - `재산 수준`
  - `직업`
  - (추가 특성: 나이, 가족 구성 등)
- 타겟(Target) 컬럼:
  - 구매할 자동차 **급(class)**

---

## 🔍 프로젝트 진행 순서

### 1. 라이브러리 불러오기
- pandas, numpy, matplotlib, seaborn, sklearn 등 import

### 2. 데이터 불러오기
- 고객 특성 데이터를 `.csv` 파일로 로드

### 3. EDA (탐색적 데이터 분석)
- 결측치 확인 및 처리
- 데이터 기본 통계치 확인 (`describe`)
- 주요 특성 분포 시각화 (ex. 성별 비율, 소득 분포)
- 타겟(차급)별 특성 차이 분석

### 4. 데이터 전처리
- 범주형 변수 인코딩 (Label Encoding / One-Hot Encoding)
- 수치형 변수 스케일링 (StandardScaler)
- 이상치 처리 (필요 시)

### 5. 모델링
- 데이터셋 분할 (train/test split)
- 분류 모델 적용:
  - Logistic Regression
  - Random Forest Classifier
  - (선택적으로 XGBoost 등 추가 실험)
- 하이퍼파라미터 튜닝 (GridSearchCV 또는 RandomizedSearchCV 사용 가능)

### 6. 성능 평가
- Accuracy (정확도) 확인
- Confusion Matrix 시각화
- Classification Report (Precision, Recall, F1-score)

### 7. 결론 및 인사이트
- 가장 좋은 성능을 보인 모델 선정
- 어떤 특성이 자동차 급 추천에 가장 영향을 미쳤는지 피처 중요도 분석

---

## 🧠 최종 요약
| 구분 | 내용 |
|:---|:---|
| 문제 유형 | 분류(Classification) 문제 |
| 입력 데이터 | 고객 특성 (성별, 소득, 재산 등) |
| 출력 데이터 | 추천할 자동차 급 (class) |
| 주요 평가 지표 | 정확도(Accuracy), F1-score |
| 활용 가능한 모델 | 로지스틱 회귀, 랜덤 포레스트, XGBoost 등 |

---

# 📢 추가로
- 고소득자에게는 고급차를 추천하고
- 소득이 낮거나 자산이 적은 경우에는 실용적인 차를 추천하는
- 실제 판매 전략에도 응용 가능한 프로젝트!
