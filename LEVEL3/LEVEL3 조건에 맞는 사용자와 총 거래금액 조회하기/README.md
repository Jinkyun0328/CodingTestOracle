### SQL문
![image1](https://user-images.githubusercontent.com/123911778/262595557-e32012c2-90c8-49b9-a5fe-1db4274a11ae.PNG)

### 문제  
![image2](https://user-images.githubusercontent.com/123911778/262595563-2b7cf4c1-c121-4716-8fd9-c14f42d2138e.PNG)

### 결과
![image3](https://user-images.githubusercontent.com/123911778/262595550-8620bef1-3e02-4f51-aef3-143aa74356cc.PNG)

### 설명
완료된 중고 거래의 총금액이 70만원 이상인 사람을 조회한다.             
USED_GOODS_BOARD에서 STATUE에 DONE이면서 PRICE의 합이 70만을 넘어가는 것을 찾는다.           
SELECT에서 A.WRITER_ID와 B.NICKNAME이 같이 나오기 때문에           
GROUP BY에도 이 두 개가 들어가야 한다.           
SUM(A.PRICE)가 70만보다 크다는 것은 그룹화 된 것의 조건이기 때문에 HAVING에 적는다.           
