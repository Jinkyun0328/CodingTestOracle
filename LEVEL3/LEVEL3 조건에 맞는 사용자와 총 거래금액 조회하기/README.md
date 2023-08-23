### SQL문
![image1](https://user-images.githubusercontent.com/123911778/262575187-235e74f0-97af-469f-9e58-76714e8680c7.PNG)

### 문제  
![image2](https://user-images.githubusercontent.com/123911778/262575192-76a237e5-ed7c-4332-8b60-b2f734b23a38.PNG)

### 결과
![image3](https://user-images.githubusercontent.com/123911778/262575194-4dc6626d-039c-486a-b74d-5f7bd290e7aa.PNG)

### 설명
조회수는 USED_GOODS_BOARD 테이블에 저장되어 있고 파일명은 used_goods_file 태이블에 저장되어 있다.       
출력하는 것은 문자열이 연결된 형태로 ORACLE에서는 '||'을 사용하여 문자열을 연결한다.       
       
USED_GOODS_BOARD에서 VIEWS 중 최댓값을 가지는 BORAD_ID의 파일주소를 출력하는 것이므로       
WHERE에서 SELECT문을 사용하여 최댓값을 구하고 이것과 VIEWS가 같은 값인 것을 출력한다.       

출력 결과 위의 2개의 파일이 출력되었다.          
