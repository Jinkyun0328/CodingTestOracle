### SQL문
![image1](https://user-images.githubusercontent.com/123911778/263132169-81722d7c-a529-48fd-9316-1da1f354aed9.PNG)

### 문제  
![image2](https://user-images.githubusercontent.com/123911778/263132173-a9854d17-1d11-4d2d-9234-a7124fd3935c.PNG)

### 결과
![image3](https://user-images.githubusercontent.com/123911778/263132176-15560c99-ec2d-4c06-b6f7-32b9152c05d8.PNG)

### 설명
둘 이상을 등록한 사람을 구한다. HOST_ID의 숫자를 COUNT을 사용하여 집계한 다음    
HAVING을 사용하여 2 이상인 HOST ID를 반환한다.     

출력하는 것이 ID, NAME, HOST_ID이고 집계하는 컬럼이 HOST_ID이므로 WHERE절에 서브쿼리를 사용하여 구현했다.     
ID와 NAME은 HOST_ID가 동일할 때 동일한 값을 가지는 것이 아니므로 GROUP BY에서 한번에 집계하지 않고      
서브쿼리를 사용하였다.         
