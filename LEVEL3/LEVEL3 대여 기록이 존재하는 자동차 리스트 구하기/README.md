### SQL문
![image1](https://user-images.githubusercontent.com/123911778/262826015-9fab05f1-2ddc-47aa-8356-84e753aa52e7.PNG)

### 문제  
![image2](https://user-images.githubusercontent.com/123911778/262826018-144aca87-f851-48e7-90d8-7157446753e1.PNG)

### 결과
![image3](https://user-images.githubusercontent.com/123911778/262826019-b368f112-2bc5-4503-8673-654c2f04793b.PNG)

### 설명
CAR_RENTAL_COMPANY_CAR 테이블과 CAR_RENTAL_COMPANY_RENTAL_HISTORY 테이블에서           
데이터를 가져오므로 A와 B를 CAR_ID를 사용하여 INNER JOIN한다.          
START_DATE가 2022년 10월이고 CAR_TYPE이 세단인 CAR_ID를 찾으면          
HISTORY에 서로 중복된 값이 출력된다. 한 번씩만 출력하려면 DISTINCT 함수를 사용하여          
중복을 제거한 채로 출력한다.          
