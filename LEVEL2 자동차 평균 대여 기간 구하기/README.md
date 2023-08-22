### SQL문
![image1](https://user-images.githubusercontent.com/123911778/262203056-bf67dfa1-3f01-44bf-811a-68b6a7c148bb.PNG)

### 문제  
![image2](https://user-images.githubusercontent.com/123911778/262203059-22b48b3d-6cba-49c6-8fc2-ab8bdbdcecba.PNG)

### 결과
![image3](https://user-images.githubusercontent.com/123911778/262203060-75861317-ea8e-4b2a-a795-c01c64fe40ce.PNG)

### 설명
테이블에서 특정 컬럼의 평균을 구하는 함수는 AVG이다. DATEDIFF(END_DATE, START_DATE)은 DATE형의 차를 구하는 함수로여기서는 END_DATE - START_DATE로 대여기간을 구하는 함수이다. 당일에 반납해도 하루의 대여 기간이 생기기 때문에 이 값에 +1을 해주고 AVG 함수를 사용하여 평균을 구한다. 이 값을 소수점 두번째 자리에서 반올림 하므로 값은 소수점 첫번째자리까지 출력된다. 따라서 ROUND 함수에 1을 입력한다.            

