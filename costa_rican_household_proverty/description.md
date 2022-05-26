## Data description

{train|test}.csv - training set

: 다수의 사람들이 한 가정의 일부가 될 수 있다. 가장의 점수만 예측하면 됨

### Core data fields

1. id: 유저별 식별자
2. Target: 순서형 변수(소득 수준)
  - 1: 극도로 가난
  - 2: 적당히 가난
  - 3: 조금 가난
  - 4: 조금도 가난하지 않음
3. idhogar: 각 가정에 대한 식별자
4. parentesco1: 이 사람이 집주인인지 여부를 알려줌

### All data fields

1. v2a1 :  월세납부
2. hacdor :  =1 침실별 과잉 수용
3. rooms :  집 안의 모든 방의 수
4. hacapo :  =1실별 과잉 수용
5. v14a :  =1 가정에 화장실 있음
6. refrig :  =1가구에 냉장고가 있는 경우
7. v18q :  태블릿 소유
8. v18q1 :  가구 소유의 태블릿 수
9. r4h1 :  12세 미만의 남성
10. r4h2 :  남성 12세 이상
11. r4h3 :  가구원수합계
12. r4m1 :  12세 이하 여성
13. r4m2 :  12세 이상 여성
14. r4m3 :  가구원 총여성
15. r4t1 :  12세 이하인 사람
16. r4t2 :  12세 이상
17. r4t3 :  가구원 합계
18. tamhog :  가구원수
19. tamviv :  가구원수
20. escolari :  다년간의 교육
21. rez_esc :  학창시절 몇년 뒤
22. hhsize :  가구 크기
23. paredblolad :  =1 외벽의 주요 재료가 블록 또는 벽돌인 경우
24. paredzocalo :  =1 외벽의 주요 재료가 소켓인 경우(목재, 아연 또는 압베스토
25. paredpreb :  =1 외벽의 주요 재료가 사전 조립 또는 시멘트인 경우
26. pareddes :  =1 외벽의 주요 소재가 폐자재일 경우
27. paredmad :  =1 외벽의 주요 재료가 목재인 경우
28. paredzinc :  =1 외벽의 주요 재료가 징크인 경우
29. paredfibras :  =1 외벽의 주요 소재가 천연섬유일 경우
30. paredother :  =1 외벽의 주요 재료가 다른 경우
31. pisomoscer :  =1 바닥의 주요 재료가 모자이크 세라믹 테라조인 경우
32. pisocemento :  =1 바닥의 주요 재료가 시멘트인 경우
33. pisoother :  =1 바닥의 주요 재료가 다른 경우
34. pisonatur :  =1 바닥의 주요 재료가 천연 재료인 경우
35. pisonotiene :  =가정에 층이 없는 경우 1개
36. pisomadera :  =1 바닥의 주요 재료가 목재인 경우
37. techozinc :  =1 지붕의 주요 재료가 금속 포일 또는 징크인 경우
38. techoentrepiso :  =1 지붕의 주요 재료가 섬유 시멘트, 메자닌인 경우
39. techocane :  =1 지붕의 주요 재료가 천연 섬유인 경우
40. techootro :  =1 지붕의 주요 재료가 다른 경우
41. cielorazo :  =1 집에 천장이 있는 경우
42. abastaguadentro :  =1 주거지 내부의 급수인 경우
43. abastaguafuera :  =1 주거지 외부에 물이 공급되는 경우
44. abastaguano :  =1 물 공급이 없는 경우
45. public :  =CNFL, ICE, ESPH/JASEC에서 나오는 전기 1개
46. planpri :  =민간 발전소에서 나오는 전기 1개
47. noelec :  =1주거지에 전기가 없음
48. coopele :  =협동조합 전기 1개
49. sanitario1 :  =1주거지에 화장실 없음
50. sanitario2 :  =하수도 또는 하수구에 연결된 화장실 1개
51. sanitario3 :  = 정화조에 연결된 화장실 1개
52. sanitario5 :  =블랙홀 또는 레트린에 연결된 화장실 1개
53. sanitario6 :  =다른 시스템에 연결된 화장실 1개
54. energcocinar1 :  =1 요리에 사용되는 주요 에너지원이 없음(주방 없음
55. energcocinar2 :  =1 전기 조리에 사용되는 주요 에너지 공급원
56. energcocinar3 :  =요리가스에 사용되는 주요 에너지 공급원 1개
57. energcocinar4 :  =1 목재 숯 조리에 사용되는 주요 에너지원
58. elimbasu1 :  =1 유조선 트럭에 의한 쓰레기 처리의 경우
59. elimbasu2 :  =1 주로 식물성 중공 또는 매립에 의한 쓰레기 처리
60. elimbasu3 :  =1 주로 불에 태워 폐기물을 처리하는 경우
61. elimbasu4 :  =1 빈 공간에 주로 던져서 쓰레기를 처리하는 경우
62. elimbasu5 :  =1 주로 강, 하천 또는 바다에 투척하여 쓰레기를 처리하는 경우
63. elimbasu6 :  =1 쓰레기 처리가 주로 다른 경우
64. epared1 :  =벽이 나쁜 경우 1
65. epared2 :  =1 벽이 정규적인 경우
66. epared3 :  =벽이 좋은 경우 1개
67. etecho1 :  =1 지붕이 나쁜 경우
68. etecho2 :  =1 지붕이 정규적인 경우
69. etecho3 :  =1 지붕이 양호한 경우
70. eviv1 :  =1 바닥이 나쁜 경우
71. eviv2 :  =1 바닥이 규칙적인 경우
72. eviv3 :  =1 바닥이 좋은 경우
73. dis :  =1 장애인일 경우
74. male :  =1 남성일 경우
75. female :  =1 여성인 경우
76. estadocivil1 :  =10세 미만인 경우 1개
77. estadocivil2 :  =자유 또는 커플링된 경우 1개
78. estadocivil3 :  =결혼한 경우 1개
79. estadocivil4 :  =이혼한 경우 1개
80. estadocivil5 :  =1 별거한 경우
81. estadocivil6 :  =과부 경우 1개
82. estadocivil7 :  =싱글일 경우 1개
83. parentesco1 :  =가정의 가장일의 경우 1개
84. parentesco2 :  =배우자/파트너일 경우 1개
85. parentesco3 :  =아들/딸일 경우 1개
86. parentesco4 :  =의붓아들/딸 일 경우
87. parentesco5 :  =법률상 아들/딸일 경우 1개
88. parentesco6 :  =손자/손자일 경우
89. parentesco7 :  =어머니/아버지인 경우
90. parentesco8 :  =법률상 아버지/어머니일 경우 1개
91. parentesco9 :  =형/동생인 경우 1개
92. parentesco10 :  =법률상 형제/자매인 경우 1개
93. parentesco11 :  =1 다른 가족 구성원의 경우
94. parentesco12 :  =1 가족이 아닌 다른 구성원의 경우
95. idhogar :  가구 수준 식별자
96. hogar_nin :  0~19세인 가구원 수
97. hogar_adul :  어른인 가구원수
98. hogar_mayor :  65세 이상인 가구원수
99. hogar_total :  가구원 총 인원수
100. dependency :  종속율
101. edjefe :  남성 가장의 수년간 교육
102. edjefa :  여성 가장의 수년간 교육
103. meaneduc :  평균 성인 교육년(18+)
104. instlevel1 :  =1 교육 수준 없음
105. instlevel2 :  =1 불완전한 초등교육
106. instlevel3 :  =1 완전한 초등교육
107. instlevel4 :  =1 불완전한 학업 2차 수준
108. instlevel5 :  =1 완전한 학문적 2차 수준
109. instlevel6 :  =1 불완전한 기술 2차 수준
110. instlevel7 :  =1 완전한 기술 2차 수준
111. instlevel8 :  =1학부 이상
112. instlevel9 :  =1 대학원 고등교육
113. bedrooms :  침실 수
114. overcrowding :  # 객실당 인원수
115. tipovivi1 :  =1자체 및 완전유급주택
116. tipovivi2 :  =1개 소유, 할부 결제
117. tipovivi3 :  =1 임대
118. tipovivi4 :  =1 불안정한
119. tipovivi5 :  =1 다른사람에게 할당된
120. computer :  =1 가구에 노트북 또는 데스크탑 컴퓨터가 있는 경우, 대여
121. television :  =1가구에 TV가 있는 경우
122. mobilephone :  =휴대전화일 경우 1
123. qmobilephone :  휴대전화 번호
124. lugar1 :  =1 지역 중심
125. lugar2 :  =1 지역 Chorotega
126. lugar3 :  =1 지역 PacÃƒÂ­fico central
127. lugar4 :  =1 지역 Brunca
128. lugar5 :  =1 지역 Huetar AtlÃƒÂ¡ntica
129. lugar6 :  =1 지역 Huetar Norte
130. area1 :  =1 조나 우르바나
131. area2 :  =2 조나 시골
132. age :  연령
133. SQBescolari :  에스코라리 제곱
134. SQBage :  나이 제곱
135. SQBhogar_total :  hogar_total 제곱
136. SQBedjefe :  에드제프 제곱
137. SQBhogar_nin :  hogar_nin 제곱
138. SQBovercrowding :  과밀 제곱
139. SQBdependency :  종속성 제곱
140. SQBmeaned :  평균 제곱
141. agesq :  나이 제곱
