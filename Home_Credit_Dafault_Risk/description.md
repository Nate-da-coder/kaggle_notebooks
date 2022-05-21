![Alt text](../image/home_credit.png)

application_train/ application_test: 대출 신청서에 대한 정보, 모든 대출은 각각 행을 갖고 있고, SK_ID_CURR이라는 피쳐로 구별됨. Training데이터에는 target이라는 변수가 있는데, 0은 대출을 갚았고, 1은 대출을 안갚은 것이다.

bureau: 고객의 신용도(다른 기관에서 얻어온 정보), 각각 이전 신용도는 bureau안에 행별로 존재한다. application 데이터에서는 하나의 대출이 여러개의 신용데이터를 가질 수 있다. (application 1대 -> bureau 다)

bureau_balance: bureau안의 이전 신용도에 대한 매달 데이터. 각 행렬은 이전 신용의 한 달에 대한 것이다. 하나의 이전 신용도는 여러개의 행을 가질 수 있다.

Previous_application: 이전 대출 신청 정보

POS_CASH_BALANCE: 판매 또는 고개들이 가진 현금 대출의 매달 데이터.

credit_card_balance: 고객들이 가진 이전 시용 카드 데이터

installments_payments: 이전 대출에 대한 지불 히스토리
