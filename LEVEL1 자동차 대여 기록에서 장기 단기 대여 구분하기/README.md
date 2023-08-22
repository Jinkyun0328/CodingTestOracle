### SQL문
![image1](https://user-images.githubusercontent.com/123911778/262186047-7b8753c6-fee8-4212-b0ff-48b087ef345c.PNG)

### 문제  
![image2](https://user-images.githubusercontent.com/123911778/262186050-4d75fddd-020d-4222-8a6b-6af25cc86b81.PNG)

### 결과
![image3](https://user-images.githubusercontent.com/123911778/262186049-ef179001-e28b-463d-83c1-857391b05ea8.PNG)

### 설명
조건이 START_DATE가 2022년 9월에 속하는 데이터이므로
WHERE에 TO_CHAR(START_DATE, 'YYYY-MM') = '2022-09'     
또는 WHERE에 TO_CHAR(START_DATE, 'YYYY-MM-DD') LIKE '2022-09%'을 사용하여 Tuple을 골라낸다.

대여기간이 30일 이상이면 장기 대여, 그렇지 않으면 단기 대여를 표시하면 컬럼을 추가한다.
CASE WHEN 문을 사용하여 조건에 따라 값을 넣었다.
END_DATE - START_DATE + 1이 30보다 크면 '장기 대여'를 넣었고 그ㅓㅀ지 않으면 '단기 대여'를 넣었다.
이 칼럼의 이름을 RENT_TYPE을 설정했다.

DATE 자료형에서 연-월-일만 출력하기 위해서는 TO_CHAR을 사용하여 출력한다.
DATE 자료형에서 특정 연도 또는 월, 일을 포함하는지 확인할 때 TO_CHAR을 사용하여 문자형으로 변경한다.
날짜와 날짜 사이의 길이를 구할 때는 DATE형 - DATE형을 사용하여 구한다.
END_DATE - START_DATE을 사용하면 날짜와 날짜 사이의 길이를 구해서 대여 기간을 구할 수 있다.
단 END_DATE와 START_DATE가 같을 때도 하루동안 대여한 것이기 때문에 이 값에 +1을 해주었다.
