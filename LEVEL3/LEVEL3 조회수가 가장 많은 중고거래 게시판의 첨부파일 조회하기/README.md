### SQL문
![image1](https://user-images.githubusercontent.com/123911778/262590161-e6ed3b76-7dee-4b92-ac28-dfdb7ab358d9.PNG)

### 문제  
![image2](https://user-images.githubusercontent.com/123911778/262590164-f7eefcf7-abec-4267-a1cd-fc628e4eccb5.PNG)

### 결과
![image3](https://user-images.githubusercontent.com/123911778/262590156-8d138c65-f0e1-43f7-a3cd-0d4546031460.PNG)

### 설명
중고 거래 게시물을 3건 이상 등록한 사용자의 데이터를 출력하려고 한다.          
ORACLE에서 문자열을 연결할 때는 || 연산자를 사용하여 연결한다.       
휴대폰 전화번호는 3, 4, 4자리로 구분지어서 중간에 -를 넣어 출력한다.       
substr 함수를 사용하여 TLNO을 잘라서 사용했다.       

게시물을 3건 이상 등록한 사용자는 where에서 query을 사용하였다.       
count 함수를 사용하여 writer_id를 기준으로 게시물의 수를 구했고 출력된 ID와 같은 ID를 가지고 있는        
user_id와 요구한 행을 출력한다.       
