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
CAR_RENTAL_COMPANY_CAR 테이블에서 OPTIONS에 네비게이션을 포함하는 데이터를 출력한다.
문자를 포함하는 여부를 확인할 때는 LIKE을 사용하고 네비게이션의 양 옆에 %_%은 앞과 뒤에 다른 문자가 올 수 있음을 나타낸다.
