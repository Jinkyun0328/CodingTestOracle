### SQL문
![image1](https://user-images.githubusercontent.com/123911778/262845827-7d80d2de-d07f-4810-8907-309fcd165637.PNG)

### 문제  
![image2](https://user-images.githubusercontent.com/123911778/262845834-789f1593-0f7d-4a0b-bd2a-1e4dd42680fd.PNG)

### 결과
![image3](https://user-images.githubusercontent.com/123911778/262845836-090f6b95-253c-474a-8a1d-63179b15f4c4.PNG)

### 설명
카테고리별로 그룹화를 한 후 판매량의 합계를 집계하려고 한다.             
BOOK과 BOOK_SALES에서 데이터를 가져왔으므로 JOIN을 사용하여 두 테이블에서 데이터를 가져온다.          
2022년 01월에 판매된 판매량의 합을 집계하므로 조건문에 날짜를 2022-01로 정한다.          
카테고리를 그룹화하고 SALES을 SUM 함수로 집계하여 출력한다.          
