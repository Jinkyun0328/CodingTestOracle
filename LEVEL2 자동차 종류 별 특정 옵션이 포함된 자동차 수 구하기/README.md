### SQL문
SELECT CAR_TYPE, COUNT(CAR_TYPE) AS CARS            
FROM CAR_RENTAL_COMPANY_CAR         
WHERE OPTIONS LIKE '%통풍시트%'         
    OR OPTIONS LIKE '%열선시트%'         
    OR OPTIONS LIKE '%가죽시트%'         
GROUP BY CAR_TYPE         
ORDER BY CAR_TYPE;         

### 문제  
![image2](https://user-images.githubusercontent.com/123911778/262203067-e70e9679-9f94-4c37-a851-8538f3df6d97.PNG)

### 결과
![image3](https://user-images.githubusercontent.com/123911778/262203069-ee017cf0-761f-4499-813c-331726d9ee99.PNG)

### 설명
'통풍시트, 열선시트, 가죽시트 중 하나 이상의 옵션이 포함된 자동자'를 먼저 구하고         
그곳에서 자동차 종류 별로 몇 대인지 출력하는 SQL문을 작성한다.         

OPTION에 통풍시트, 열선시트, 가죽시트 중 하나라도 포함하는 것. LIKE를 사용하고 OR로 연결  
자동차 종류별로 몇 대인이 출력하는 것이므로 COUNT 함수는 CAR_TYPE에 따라 묶어준다.  
