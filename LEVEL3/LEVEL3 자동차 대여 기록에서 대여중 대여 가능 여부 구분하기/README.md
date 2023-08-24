### SQL문
![image1](https://user-images.githubusercontent.com/123911778/262828557-b1bd0912-d045-4432-8714-115ad643e7f4.PNG)

### 문제  
![image2](https://user-images.githubusercontent.com/123911778/262828559-f42aa95a-764b-4104-896b-68d9b8bb3d39.PNG)

### 결과
![image3](https://user-images.githubusercontent.com/123911778/262828560-dfcc60c1-8fa3-41de-8e7c-4a3fad53c2a8.PNG)

### 설명
테이블에서 START_DATE가 22년 10월 16일보다 작거나 같으면서 END_DATE가 22년 10월 16일보다 큰 것을 찾아        
'대여중'이라고 출력한다. 그렇지 않으면 '대여 가능'이라고 출력한다.      
이것을 case when then 문으로 작성했다.      

FROM에서 서브쿼리를 사용하여 car_id와 대여중, 대여 가능을 출력하는 availability 테이블을 받아왔다.      
history를 보면 하나의 car_id는 한 번만 대여한 것이 아닌 10월 16일 이전이나 이후에도 대여 기록이 있다.      
이전 데이터에서는 대여 가능이라고 나온다고 하더라도 10월 16일과 겹치는 부분이 한 번이라도 있으면      
대여중이라고 출력해야 한다. 중복을 없애면서 대여중을 대여 가능보다 더 우선시 하고 있으므로      
car_id를 group by로 묶고 max를 사용하여 출력한다.      
대여중이 대여 가능보다 가나다 순서에서 뒤에 있으므로 max를 출력하면 하나라도 대여중이 있으면      
대여중이 출력된다.      
