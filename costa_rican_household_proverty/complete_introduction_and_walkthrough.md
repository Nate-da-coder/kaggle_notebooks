# 문제 풀이

: household의 poverty level을 맞추는 multil-class classification

### Metric

: Macro F1 = (F1 class 1 + F1 class 2 + F1 class 3 + F1 class 4) / 4

F1 = 2 * (precision * recall)/(precision + recall)

**precision(정밀도)**

: Positive로 예측한 경우, 실제로 Positive인 비율. 즉 예측값이 얼마나 정확한지를 알려준다.

TP / (TP + FP)

이메일에서 스팸메일이 있는데(Negative) 그것을 못 맞췄을 때(Postive) 패널티를 부여받는 지표

**recall(재현율)**

: 실제 Positive인 것 중, 올바르게 Positive라고 맞춘 비율

TP / (TP + FN)

암 환자(Positive)를 암 환자가 아니라고(Negative) 예측할 때 패널티를 부여받는 지표

### Roadmap

1. 문제 이해
2. EDA
- int, object, flaot형 변수별로 Target그룹으로 데이터 분석
- Label 오류 확인
- Missing Value 처리(관련 있는 변수와 비교하여 왜 Missing일지를 고민)
- 두개의 obejct 카테고리 변수의 관계성을 보여주는 그래프 생성
- missing value를 변수로 처리해서(0 or 1) Target에 분포가 다른지 확인
3. 피쳐엔지니어링
- 집에 사는 사람들의 데이터를 agg
- household 데이터와 merge
- squared variables(linear 모델이 non-linear한 관계를 학습하는데는 좋다.)를 제거 복잡한 모델에서는 불필요하다. 복잡한 모델에서는 non-squared한 데이터들과 강하게 상관관계를 가진다.
- household데이터중 변수간에 0.95이상의 상관관계를 가지는 것은 데이터를 보고 제거하도록 한다.
- creating ordinal variable
  - 어떤 유형의 전기를 사용사용하는지
  - 벽의 상태를 보여주는
  - 지붕의 상태를 보여주는
  - 벽+지붕+바닥 변수를 모두 합친 것
  - warning 변수 생성(화장실 없음 + 층이 없음 + 물 공급없음 + 천장 없음)
  - bonus 변수 생성(냉장고 + 컴퓨터 + 태블릿 + tv)
  - 가구원 수 대비 휴대폰 수
  - 가구원 수 대비 태블릿 수
  - 가구원 수 대비 방 수
  - 가구원 수 대비 렌트비용
  - pearson correlation vs spearman correlation
  - 새로 생성한 feature와 target과의 관계확인
  - male제거
  - 다년간의 교육 / 나이
  - 교육 수준 / 나이
  - 태블릿 + 모바일
  - idhogar그룹별로 agg (새로운 지표 생성방법: range_)
  - feature selection(correlation > 0.95)
  - Target과 corr이 높은 데이터를 그래프로 확인
4. 몇개의 베이스라인 모델과 비교
5. 복잡한 머신러닝 모델 시도
6. 모델 최적화
7. 모델 예측에 대한 평가
8. 결론
