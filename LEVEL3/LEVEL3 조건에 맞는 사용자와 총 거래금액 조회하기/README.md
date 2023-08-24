### SQL문
![image1](https://user-images.githubusercontent.com/123911778/262595557-e32012c2-90c8-49b9-a5fe-1db4274a11ae.PNG)

### 문제  
![image2](https://user-images.githubusercontent.com/123911778/262595563-2b7cf4c1-c121-4716-8fd9-c14f42d2138e.PNG)

### 결과
![image3](https://user-images.githubusercontent.com/123911778/262595550-8620bef1-3e02-4f51-aef3-143aa74356cc.PNG)

### 설명
완료된 중고 거래의 총금액이 70만원 이상인 사람을 조회한다.           
합을 구할 때는 GROUP BY를 사용하여 그룹을 만들고 집계함수 SUM을 사용하여 합을 구한다.           
SELECT에 WRITER_ID와 NICKNAME이 출력되기 때문에 GROUP BY에도 이 두 가지를 사용하여 그룹화를 한다.           
PRICE의 합을 TOTAL_SALES로 출력하고 이 값이 700000 이상인 그룹을 출력하는데           
그룹화된 데이터의 조건문은 WHERE이 아닌 HAVING에 작성한다.           
