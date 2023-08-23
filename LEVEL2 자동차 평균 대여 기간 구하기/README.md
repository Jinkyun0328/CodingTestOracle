### SQL문
![image1](https://user-images.githubusercontent.com/123911778/262203056-bf67dfa1-3f01-44bf-811a-68b6a7c148bb.PNG)

### 문제  
![image2](https://user-images.githubusercontent.com/123911778/262203059-22b48b3d-6cba-49c6-8fc2-ab8bdbdcecba.PNG)

### 결과
![image3](https://user-images.githubusercontent.com/123911778/262203060-75861317-ea8e-4b2a-a795-c01c64fe40ce.PNG)

### 설명
CAR_ID 별로 대여 기간의 평균을 구하려고 한다.          
Column의 평균은 AVG 함수를 사용하여 구할 수 있다.         
단 GROUP BY를 하지 않으면 모든 Column에 대해 평균값을 구하기 때문에         
이 문제처럼 CAR_ID 별로 평균을 구하고 싶으면 CAR_ID로 그룹화해야 한다.         

GROUP BY를 사용했을 때는 조건문으로 WHERE 대신 HAVING을 사용한다.         
평균대여기간이 7일 이상인 것만 출력하려고 한다.         
그럼 HAVING에서 AVERAGE_DURATION이 7보다 크다라는 조건을 붙여준다.         

DATEDIFF은 날짜형 자료형 간의 차이를 구하는 함수         
AVG 컬럼의 평균을 구하는 함수         
ROUND 반올림         

