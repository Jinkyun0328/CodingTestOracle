### SQL문
![image1](https://user-images.githubusercontent.com/123911778/262521205-66bca1af-cdb4-4760-8505-c1fa7bc3c562.PNG)

### 문제  
![image2](https://user-images.githubusercontent.com/123911778/262521209-e6b5a884-6ff7-4214-9f03-228aec399d2d.PNG)

### 결과
![image3](https://user-images.githubusercontent.com/123911778/262521210-e9da7b25-1daa-46ec-a2e2-e28a12d14bf9.PNG)

### 설명
보호소에서 몇 시에 입양이 가장 활발하게 일어나는지 알아보려고 한다.
각 시간대별로 입양이 몇 건이나 발생했는지 조회하려고 한다.

FROM에서 서브쿼리를 사용하여 09-11-22 11:22:33으로 출력되는 DATE형을 char형으로 변환하였고
'FMHH24'를 넣어서 시간만을 추출한 후 숫자형으로 변경했다.   
그럼 hour에는 시간을 나타내는 정수가 저장된다.   

count 함수를 사용하여 hour을 기준으로 카운트하여 출력했고 9시부터 19시 59분까지 발생한 입양을 조회하는 것이므로
having에 between 함수를 사용하여 조건을 추가한다.    
