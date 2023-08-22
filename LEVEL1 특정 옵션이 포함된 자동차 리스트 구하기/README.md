### SQL문
SELECT       
CAR_ID,      
CAR_TYPE,      
DAILY_FEE,      
OPTIONS     
FROM CAR_RENTAL_COMPANY_CAR      
WHERE OPTIONS LIKE '%네비게이션%'     
ORDER BY CAR_ID DESC     
;     

### 문제  
![image1](https://user-images.githubusercontent.com/123911778/262185279-70c7e6e8-4d95-47a4-9202-281d64000932.PNG)

### 결과
![image2](https://user-images.githubusercontent.com/123911778/262185283-ac789110-bc5c-4b9c-8575-526018ad1c32.PNG)

### 설명
2개의 Table에서 데이터를 가져올 때는 테이블 명에 별칭을 붙여서 사용한다.
여기서는 USED_GOODS_BOARD 테이블에 A, USED_GOODS_REPLY 테이블에 B라는 별칭을 붙였다.
조건문을 나타내는 WHERE에서 A와 B에서 동시에 가지고 있는 Column인 Board_id가 서로 같다고 명시해주었고
SELECT에서는 어떤 테이블의 Column을 가져 왔는지 A.TITLE, B.REPLY_ID 등의 방식으로 명시한다.
A.CREATED_DATE에는 DATE 자료형이 저장되어 있는데 2022년 10월의 데이터를 가져오기 위해서
TO_CHAR을 사용하여 DATE 자료형을 CHAR 자료형으로 변환하였고 앞의 연도와 달까지만 가져와서 '2022-10'과 비교했다.
ORDER BY은 정렬을 하는 구문으로 먼저 B.CREATED_DATE에 대해 오름차순으로 정렬하고 같은 값이 있을 경우  
A.TITLE에 대해 오름차순으로 정렬한다.
