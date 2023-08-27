### SQL문
![image1](https://user-images.githubusercontent.com/123911778/263148569-dd15120b-a89c-429d-b15a-fa58c03c88de.PNG)

### 문제  
![image2](https://user-images.githubusercontent.com/123911778/263148571-08146e52-cf59-4d20-a13c-5a32dc734599.PNG)

### 결과
![image3](https://user-images.githubusercontent.com/123911778/263148572-810b2deb-ec2e-4b4c-871c-f3439c52a1c5.PNG)

### 설명
식품분류별로 가격이 제일 비싼 식품의 정보를 조회하려고 한다.         
식품분류와 가장 비싼 가격 이외에도 PRODUCT_NAME이 들어가기 때문에 GROUP BY로 한 번에 집계할 수 없다.         

FROM의 서브쿼리를 사용하여 CATEGORY별로 PRICE의 MAX값을 출력하였고 FOOD_PRODUCT 테이블과         
CATEGORY로 INNER JOIN했다. CATEGORY가 과자, 국, 김치, 식용유이면서 PRICE가 MAX_PRICE와 같은 튜블을 출력했다.           
