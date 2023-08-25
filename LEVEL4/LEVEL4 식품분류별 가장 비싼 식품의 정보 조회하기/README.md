### SQL문
![image1](https://user-images.githubusercontent.com/123911778/263141534-ca05f603-c06c-433b-b298-6ec20916b38c.PNG)

### 문제  
![image2](https://user-images.githubusercontent.com/123911778/263141537-8994fff9-ac49-4633-a099-4d663e660929.PNG)

### 결과
![image3](https://user-images.githubusercontent.com/123911778/263141540-6c5cc01a-a7fd-4b61-8235-5eba20269860.PNG)

### 설명
보호소에서 각 시간별로 입양이 몇 건이나 발생했는지 조회하려고 한다.        
날짜형 자료형에서 시간만을 출력할 때는 TO_CHAR을 사용하고 HH24를 넣으면 24시간으로 출력할 수 있다.        
시간을 GROUP BY에 넣어서 COUNT 하여 시간별로 입양이 발생한 횟수를 구할 수 있다.        

문제에서는 0부터 23까지 시간별로 출력하기를 요구하고 있기 때문에        
0부터 23까지가 저장된 행이 있어야 한다.        
LEVEL-1을 출력하여 0부터 23까지출력하고 이 테이블을 횟수를 구한 테이블과 OUTER JOIN으로 연결하여 출력한다.         
