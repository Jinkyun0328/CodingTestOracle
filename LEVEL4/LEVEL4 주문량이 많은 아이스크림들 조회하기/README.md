### SQL문
![image1](https://user-images.githubusercontent.com/123911778/263862169-27b7c5da-c70e-480e-954f-b63f57ede278.PNG)

### 문제  
![image2](https://user-images.githubusercontent.com/123911778/263862145-f5aaa871-785b-4ae5-9bb2-09840933ea93.PNG)

### 결과
![image3](https://user-images.githubusercontent.com/123911778/263862147-ee0b8775-23a1-4a95-8235-abe103fc5477.PNG)

### 설명
PRODUCT_DATE가 2022년 5월인 식품들의 총매출을 조회한다.                        
PRICE는 FOOD_PRODUCT 테이블에 저장되어 있고 식품의 양과 생산일자 등의 주문리스트는 FOOD_ORDER에 저장되어 있다.                        
두 개의 테이블에서 데이터를 가져오기 때문에 JOIN을 사용한다.                        
두 개의 테이블에 동시에 들어있는 컬럼인 PRODUCT_ID을 서로 동일한 값으로 설정하여 INNDER JOIN을 실시한다.                        

FOOD_ORDER 테이블에서 같은 식품ID를 가지는 물품을 중복하여 주문할 수 있다.                        
총 매출을 구하기 위해서는 PRODUCT_ID로 그룹화하고 PRICE와 AMOUNT의 곱의 합을 구한다.                        

SELECT에서 PRODUCT_ID와 PRODUCT_NAME을 조회하는데 GROUP BY를 사용할 때는                        
SELECT에 있는 컬럼이 GROUP BY에도 들어가 있어야 한다.                        
PRODUCT_NAME은 PRODUCT_ID마다 하나씩 들어있기 때문에 같이 묶어서 사용할 수 있다.                          


