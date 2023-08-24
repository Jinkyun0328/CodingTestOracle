### SQL문
![image1](https://user-images.githubusercontent.com/123911778/262841432-7028a3c2-d8f0-4cf2-a827-393282aa3f47.PNG)

### 문제  
![image2](https://user-images.githubusercontent.com/123911778/262841439-a0f9534a-dadb-4a5d-8bf3-486a0ee03a0f.PNG)

### 결과
![image3](https://user-images.githubusercontent.com/123911778/262841446-a496314a-2cb5-46a9-bdfa-7852a38c8ea4.PNG)

### 설명
8월부터 10월까지 전체 대여 횟수가 5회 이상인 CAR_ID에 대하여 각 월별로 car_id의 대여 횟수를 출력한다.              
WHERE문에서 서브쿼리를 사용하여 8월 부터 10월까지 대여 횟수가 5회 이상인 CAR_ID만 가져왔고              
월, CAR_ID를 그룹으로 묶은 후 COUNT 함수를 사용하여 집계했다.                

EXTRACT 함수는 날짜형 자료형에서 연, 월, 일을 추출할 수 있는 함수로              
MONTH FROM START_DATE을 사용하여 START_DATE에서 월을 가져올 수 있다.              
