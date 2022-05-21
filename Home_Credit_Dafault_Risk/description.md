# Data Description

<img src="./image/home_credit.png"  title="table description"/>

application_train/ application_test: 대출 신청서에 대한 정보, 모든 대출은 각각 행을 갖고 있고, SK_ID_CURR이라는 피쳐로 구별됨. Training데이터에는 target이라는 변수가 있는데, 0은 대출을 갚았고, 1은 대출을 안갚은 것이다.

bureau: 고객의 신용도(다른 기관에서 얻어온 정보), 각각 이전 신용도는 bureau안에 행별로 존재한다. application 데이터에서는 하나의 대출이 여러개의 신용데이터를 가질 수 있다. (application 1대 -> bureau 다)

bureau_balance: bureau안의 이전 신용도에 대한 매달 데이터. 각 행렬은 이전 신용의 한 달에 대한 것이다. 하나의 이전 신용도는 여러개의 행을 가질 수 있다.

Previous_application: 이전 대출 신청 정보

POS_CASH_BALANCE: 판매 또는 고개들이 가진 현금 대출의 매달 데이터.

credit_card_balance: 고객들이 가진 이전 시용 카드 데이터

installments_payments: 이전 대출에 대한 지불 히스토리

### application_{train|test}

1. SK_ID_CURR: ID of loan 대출 ID
2. TARGET: Target Variable(0: 대출을 갚은 경우, 1: 대출 지불에 어려움을 겪는 경우)
3. -
4. -
5. NAME_CONTRACT_TYPE: 대출이 현금인지 리볼빙인지(리볼빙: 약정된 결제일에 최소 금액만 결제하고 나머지 대금은 대출로 이전하는 방식)
6. CODE_GENDER: 성별
7. FLAG_OWN_CAR: 차 소유 여부
8. FLAG_OWN_REALTY: 집/아파트 소유 여부
9. CNT_CHILDREN: 자녀 수
10. AMT_INCOME_TOTAL: 수입
11. AMT_CREDIT: 대출 총액
12. AMT_ANNUITY: 매달 내야하는 돈(이자 포함)
13. AMT_GOODS_PRICE: 대출받아서 사려고한 상품 총액
14. NAME_TYPE_SUITE: 대출 신청시 동행인
15. NAME_INCOME_TYPE: 소득 타입
16. NATE_EDUCATION_TYPE: 최종 학력 수준
17. NAME_FAMILY_STATUS: 가족 현황
18. NAME_HOUSING_TYPE: 주거 현황
19. REGION_POPULATION_RELATIVE: 고객 거주 지역의 정규화된 인구수
20. DAYS_BIRTH: 신청날 고객 나이
21. DAYS_EMPLOYED: 신청일 기준 현재 직장에서 일한 일 수
22. DAYS_REGISTRATION: 신청일 기준고객이 등록서류를 변경한 일 수
23. DAYS_ID_PUBLISH: 고객이 대출을 신청한 동안에 신분증 문서를 변경한 일 수
24. OWN_CAR_AGE: 고객 자동차 연식
25. FLAG_MOBILE: 고객 휴대폰 번호 제공 여부
26. FALG_EMP_PHONE: 고객 직장 번호 제공 여부
27. FLAG_WORK_PHONE: 고객 자택 번호 제공 여부
28. FLAG_CONT_MOBILE: 고객 휴대폰 연결 가능 여부
29. FLAG_PHONE: 고객 자택 번호 제공 여부
30. FLAG_EMAIL: 고객 이메일 제공 여부
31. OCCUPATION_TYPE: 고객 직업
32. CNT_FAM_MEMBERS: 고객 가족 구성원 수
33. REGION_RATING_CLIENT: 고객이 사는 지역에 대한 우리의 평가
34. REGION_RATING_CLIENT_W_CITY: 고객이 사는 도시에 대한 우리의 평가
35. WEEKDAY_APPR_PROCESS_START: 대출 신청 요일
36. HOUR_APPR_PROCESS_START: 대출 신청한 대략적인 시각
37. REG_REGION_NOT_LIVE_REGION: 고객 영구 주소와 흭득 주소가 일치하는지
38. REG_REGION_NOT_WORK_REGION: 고객 영구 주소와 직장 주소가 일치하는지
39. LIVE_REGION_NOT_WORK_REGION: 고객 흭득 주소와 직장 주소가 일치하는지
40. REG_CITY_NOT_LIVE_CITY: 고객 영구 주소와 흭득 주소가 일치하는지
41. REG_CITY_NOT_WORK_CITY: 고객 영구 주소와 직장 주소가 일치하는지
42. LIVE_CITY_NOT_WORK_CITY: 고객 흭득 주소와 직장 주소가 일치하는지
43. ORGANIZATIION_TYPE: 고객이 일하는 조직의 유형
44. EXT_SOURCE_1: 외부 데이터 소스의 정규화된 점수
45. EXT_SOURCE_2
46. EXT_SOURCE_3
47. ~ 고객이 거주하는 곳에 대한 표준화된 정보, 아파트 사이즈, 공용지, 주거지, 빌딩 나이, 엘리베이터 수, 입구 수, 빌딩 상태, 층 수 등에 대한 평균, 최빈 값, 중앙 값
94. OBS_30_CNT_SOCIAL_CIRCLE: 고객 주위 사람 중 30일 이상 지불이 늦을 수 있는 사람의 수
95. DEF_30_CNT_SOCIAL_CIRCLE: 고객 주위 사람 중 30일 이상 지불이 정말 늦은 사람의 수
96. OBS_60_CNT_SOCIAL_CIRCLE: 고객 주위 사람 중 60일 이상 지불이 늦을 수 있는 사람의 수
97. DEF_60_CNT_SOCIAL_CIRCLE: 고객 주위 사람 중 60일 이상 지불이 정말 늦은 사람 수
98. DAYS_LAST_PHONE_CHANGE: 대출 신청 며칠 전에 휴대폰을 변경했는가?
99. ~ 고객 문서 제공 횟수
119. AMT_REQ_CREDIT_BUREAU_HOUR: 신청전 1시간동안 고객에 대한 CB로의 문의 횟수
120. AMT_REQ_CREDIT_BUREAU_DAY: 신청 전 하루동안 고객에 대한 CB로의 문의 횟수
121. AMT_REQ_CREDIT_BUREAU_WEEK: 신청 전 일주일동안 고객에 대한 CB로의 문의 횟수
122. AMT_REQ_CREDIT_BUREAU_MON: 신청 전 한 달동안 고객에 대한 CB로의 문의 횟수
123. AMT_REQ_CREDIT_BUREAU_QRT: 신청 전 세달 동안 고객에 대한 CB로의 문의 횟수
124. AMT_REQ_CREDIT_BUREAU_YEAR: 신청 전 일년동안 고객에 대한 CB로의 문의 횟수
