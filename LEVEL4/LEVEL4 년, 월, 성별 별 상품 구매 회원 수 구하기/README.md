### SQL문
![image1](https://user-images.githubusercontent.com/123911778/263872584-95436b20-b083-47cd-8f3c-e458cec74110.PNG)

### 문제  
![image2](https://user-images.githubusercontent.com/123911778/263872595-b696f92b-8023-4953-91ef-8647dbc56179.PNG)

### 결과
![image3](https://github.com/Jinkyun0328/CodingTestOracle/issues/41)

### 설명
오라클에서 날짜형 자료형의 년, 월, 일을 추출하는 함수는 EXTRACT()이다.            
USER_INFO 테이블과 ONLINE_SALE 테이블을 JOIN하여 데이터를 가져오고            
GENDER가 NULL이 아닌 행을 가져온다.            
연, 월, 성별마다 유저의 수를 조회하는 것이므로            
YEAR, MONTH, GENDER을 GROUP BY로 묶고 COUNT을 사용하여 숫자를 센다.            
여기서 동일한 유저가 물건을 다수 구매했을 수 있으므로 DISTINCT을 사용하여 중복을 제거해준다.              
