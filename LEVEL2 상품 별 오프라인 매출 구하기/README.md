### SQL문
FROM OFFLINE_SALE OS INNER JOIN PRODUCT PR     
ON OS.PRODUCT_ID = PR.PRODUCT_ID      
GROUP BY PR.PRODUCT_CODE   
ORDER BY SUM(OS.SALES_AMOUNT * PR.PRICE) DESC, PR.PRODUCT_CODE;   

### 문제  
![image2](https://user-images.githubusercontent.com/123911778/262529963-69392fd5-7610-4aab-8682-c1145897b60d.PNG)

### 결과
![image3](https://user-images.githubusercontent.com/123911778/262529979-843b7f5a-c0d9-450a-a572-b0fcfff4aeb3.PNG)

### 설명
상품 별 매출액 합계를 출력하려고 한다.   
