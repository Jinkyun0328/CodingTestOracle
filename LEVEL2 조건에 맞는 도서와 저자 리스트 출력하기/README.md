### SQL문
![image1](https://user-images.githubusercontent.com/123911778/262203070-171875c4-c09f-4d60-8b12-526b14112887.PNG)

### 문제  
![image2](https://user-images.githubusercontent.com/123911778/262203071-f760789c-14ab-4c4d-8aea-f71644ae3827.PNG)

### 결과
![image3](https://user-images.githubusercontent.com/123911778/262203074-4225338f-8400-4199-8cca-9ce2e68f0115.PNG)

### 설명
도서의 정보를 저장하고 있는 BOOK 테이블과 저자의 정보를 저장하고 있는 AUTHOR 테이블의 정보를 join해서 사용한다.         
BOOK과 AUTHOR에는 공동적으로 AUTHOR_ID를 가지고 있으므로        
A의 AUTHOR_ID와 B의 AUTHOR_ID가 서로 같다는 것을 WHERE절에서 명시해준다.        
서로 교집합인 데이터만을 JOIN하는 것을 inner join이라고 하고 따로 (+) 표시나 join 표시를 하지 않는다.       
       
CATEGORY가 경제인 튜플을 찾고       
출판연도를 연, 월, 일까지만 출력하려고 하기 때문에 TO_CHAR을 사용하여 출력한다.        
