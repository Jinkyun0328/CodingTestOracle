### SQL문
![image1](https://user-images.githubusercontent.com/123911778/262509180-766717fd-9ae4-4ece-b61d-c5a7b16e8c28.PNG)

### 문제  
![image2](https://user-images.githubusercontent.com/123911778/262509181-4325fe94-5f2f-4b87-aea1-5e3468e61c22.PNG)

### 결과
![image3](https://user-images.githubusercontent.com/123911778/262509183-9fd072e1-538f-4d32-8c7e-769732813f81.PNG)

### 설명
중복되는 이름을 가진 동물의 수를 찾는다.       
횟수를 찾는 것은 COUNT 함수를 사용하여 진행하고      
NAME별로 횟수를 세는 것이기 때문에 NAME으로 그룹화한다.      
중복이 되는 이름을 찾기 때문에 조건에서 1보다 큰 값을 찾는다.      
그룹화 한 것에 대한 조건문은 WHERE이 아닌 HAVING에 명시한다.      
