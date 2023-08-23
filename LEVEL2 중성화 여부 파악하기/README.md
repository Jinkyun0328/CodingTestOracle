### SQL문
![image1](https://user-images.githubusercontent.com/123911778/262509640-0fbb0420-5529-43df-88b1-db8ec87cac79.PNG)

### 문제  
![image2](https://user-images.githubusercontent.com/123911778/262509641-b3dfa5d8-6fc8-4662-b412-5589ddde9ef7.PNG)

### 결과
![image3](https://user-images.githubusercontent.com/123911778/262509643-cb06d9eb-d9c0-4bf5-a368-2b790642d214.PNG)

### 설명
중성화 여부를 파악하려고 한다. 중성화된 동물은 Neutered 또는 Sparyed를 포함하고 있다.         
SEX_UPON_INTAKE에 위의 단어가 포함되어 있는지를 물어보는 것이기 때문에        
LIKE를 사용하여 포함되어 있는지의 여부를 판단하고        
CASE WHEN THEN 문을 사용하여 포함되어 있는 경우 O를 출력하고 아니면 X를 출력한다.        
