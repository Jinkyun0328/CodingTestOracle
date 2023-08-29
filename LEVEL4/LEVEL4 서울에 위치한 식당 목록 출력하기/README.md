### SQL문
![image1](https://user-images.githubusercontent.com/123911778/263865177-1a863fa0-94a4-4c36-a8dd-c729c2a3fedf.PNG)

### 문제  
![image2](https://user-images.githubusercontent.com/123911778/263865179-7f89143e-5181-4db0-86b9-30e29e7e9c95.PNG)

### 결과
![image3](https://user-images.githubusercontent.com/123911778/263865172-65100572-2b3c-41fb-8843-0ddea382d36b.PNG)

### 설명
리뷰 평균점수의 소수점 둘째자리까지 출력하려고 한다.                 
조회하고자 하는 정보인 REST_ID, REST_NAME, FOOD_TYPE, FAVORITES, ADDRESS은 REST_INFO 테이블에 들어있고             
리뷰 점수인 REVIEW_SCORE은 REST_REVIEW 테이블에 들어있다.             

두 개의 테이블에서 데이터를 가져오므로 JOIN을 사용하여 테이블을 가여돈다.             
A와 B에 모두 있는 컬럼인 REST_ID을 같다고 설정하여 INNER JOIN을 하고             
리뷰 점수의 평균은 집계함수 AVG을 사용하여 출력한다.             

REST_ID가 하나로 정해지면 REST_NAME, FOOD_TYPE, FAVORITES, ADDRESS 등은 하나의 값을 가지기 때문에             
GROUP BY에서 묶어서 사용할 수 있다. GROUP BY을 사용할 때 SELECT에서 조회하는 컬럼은 GROUP BY에도 있어야 한다.             

