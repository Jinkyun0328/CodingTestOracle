### SQL문
![image1](https://user-images.githubusercontent.com/123911778/263134966-3ec20d49-4dad-45e5-8750-89e87e4b0671.PNG)

### 문제  
![image2](https://user-images.githubusercontent.com/123911778/263134970-aead7660-bfea-4b75-b7ac-d38f428c18e5.PNG)

### 결과
![image3](https://user-images.githubusercontent.com/123911778/263134971-ddeef3df-9848-478a-a22e-584e1d1bf6f9.PNG)


### 설명
보호 시작일과 입양일을 모두 알아야 하므로 INS와 OUT 테이블에서 데이터를 가져온다.      
INNER JOIN을 사용하여 두 테이블에서 데이터를 가져오고    
INS의 DATETIME이 OUTS의 DATETIME보다 큰 행을 출력한다.    
