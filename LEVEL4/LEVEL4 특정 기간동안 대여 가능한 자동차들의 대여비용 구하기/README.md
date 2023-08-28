### SQL문
![image1]()

### 문제  
![image2]()

### 결과
![image3]()

### 설명
CAR_RENTAL_COMPANY_CAR 테이블에는 CAR_TYPE과 하루요금, 옵션 등이 저장되어 있다.
CAR_RENTAL_COMPANY_RENTAL_HISTORY 테이블에는 CAR_ID별로 대여시작 날짜와 대여종료 날짜가 저장되어 있다.
CAR_RENTAL_COMPANY_DISCOUNT_PLAN 테이블에는 CAR_TYPE 별로 7, 30, 90일 이상일 때의 할인율이 저장되어 있다.

문제 : CAR_TYPE이 '세단' 또는 'SUV'인 자동차 중 2022년 11월 1일부터 2022년 11월 30일까지 대여가능한 자동차를 고른다.
일일 대여 요금에 자동차 종류별 대여기간이 30일 이상인 경우의 할인율을 적용하여 30일간의 대여 금액을 구한다.
대여 금액이 50만원 이상 200만원 미만이 되는 경우 이 금액을 출력한다.
정렬은 대여 금액, 자동차 종류, 자동차 ID를 기준으로 정렬한다.

첫번째로 대여가능한 자동차를 구해보자.
이전에 LEVEL3에서 유사한 문제를 해보았는데 대여중과 대여가능을 모두 표시한 다음 MAX를 취하는 것으로 구했었다.
대여중인 경우 WHERE에서 START_DATE가 11이거나 END_DATE가 11이거나 START_DATE가 11보다 작은데 END_DATE가 11보다 큰 경우이다.

첫번째 SELECT문
대여중으로 표시되는 CAR_ID를 출력해보자.

SELECT DISTINCT CAR_ID
FROM CAR_RENTAL_COMPANY_RENTAL_HISTORY 
WHERE TO_CHAR(START_DATE, 'YYYY-MM') = '2022-11'
    OR TO_CHAR(END_DATE, 'YYYY-MM') = '2022-11'
    OR (TO_CHAR(START_DATE, 'YYYY-MM') < '2022-11'
       AND TO_CHAR(END_DATE, 'YYYY-MM') > '2022-11')
ORDER BY CAR_ID ASC;

두번째 SELECT문
CAR_TYPE이 세단 또는 SUV인 CAR_ID 출력하기

SELECT CAR_ID, DAILY_FEE
FROM CAR_RENTAL_COMPANY_CAR  
WHERE CAR_TYPE IN ('세단', 'SUV')
    AND CAR_ID NOT IN (SELECT DISTINCT CAR_ID
                        FROM CAR_RENTAL_COMPANY_RENTAL_HISTORY 
                        WHERE TO_CHAR(START_DATE, 'YYYY-MM') = '2022-11'
                            OR TO_CHAR(END_DATE, 'YYYY-MM') = '2022-11'
                            OR (TO_CHAR(START_DATE, 'YYYY-MM') < '2022-11'
                               AND TO_CHAR(END_DATE, 'YYYY-MM') > '2022-11'))
;

세번째 SELECT문
DAILY_FEE와 30, DISCOUNT_RATE을 곱한 값
즉 CAR_RENTAL_COMPANY_CAR 와 CAR_RENTAL_COMPANY_DISCOUNT_PLAN 을 JOIN
JOIN 조건은? CAR_TYPE의 일치
WHERE의 조건? DURATION_TYPE의 값이 '30일 이상'

SELECT A.CAR_ID, A.CAR_TYPE, 
    ROUND(A.DAILY_FEE * 30 * (100 - C.DISCOUNT_RATE)/100, 0) AS FEE
FROM CAR_RENTAL_COMPANY_CAR A INNER JOIN CAR_RENTAL_COMPANY_DISCOUNT_PLAN C
    ON (A.CAR_TYPE = C.CAR_TYPE)
WHERE A.CAR_TYPE IN ('세단', 'SUV')
    AND C.DURATION_TYPE = '30일 이상'
    AND (A.DAILY_FEE * 30 * (100 - C.DISCOUNT_RATE)/100 >= 500000
        AND A.DAILY_FEE * 30 * (100 - C.DISCOUNT_RATE)/100 < 2000000)
    AND A.CAR_ID NOT IN (SELECT DISTINCT CAR_ID
                        FROM CAR_RENTAL_COMPANY_RENTAL_HISTORY 
                        WHERE TO_CHAR(START_DATE, 'YYYY-MM') = '2022-11'
                            OR TO_CHAR(END_DATE, 'YYYY-MM') = '2022-11'
                            OR (TO_CHAR(START_DATE, 'YYYY-MM') < '2022-11'
                               AND TO_CHAR(END_DATE, 'YYYY-MM') > '2022-11'))
ORDER BY 3 DESC, 2 ASC, 1 DESC
;



