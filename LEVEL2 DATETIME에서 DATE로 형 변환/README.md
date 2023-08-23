### SQL문
![image1](https://user-images.githubusercontent.com/123911778/262521213-20dea186-4779-46df-af95-af41f40368a3.PNG)

### 문제  
![image2](https://user-images.githubusercontent.com/123911778/262521216-5d1ac794-1697-41f4-be08-4ed1a215941f.PNG)

### 결과
![image3](https://user-images.githubusercontent.com/123911778/262521217-577eb887-f686-47ae-aedb-a0a4b7468952.PNG)

### 설명
DATETIME에는 날짜형으로 데이터가 저장되어 있다. 이것을 TO_CHAR을 사용하여 문자형으로 변환할 수 있는데   
날짜형의 YYYY-MM-DD HH:MI:SS를 연, 월, 일만 출력하고자 한다.                  

기타 변환법
to_char(sysdate, 'YYYY-MM-DD') : 연, 월, 일까지만 출력               
to_char(sysdate, 'YYYY-MM-DD HH:MI:SS') : 시간까지 출력               
to_char(sysdate, 'YYYY-MM-DD HH24:MI:SS') : 24시간으로 출력               
to_char(sysdate, 'YYYY-MM-DD PM HH:MI:SS') : 오후가 붙음               
to_char(sysdate, 'YYYY-MM-DD (DY)') : 요일이 붙음 예시 (화)               
to_char(sysdate, 'YYYY-MM-DD (DAY)') : 요일이 붙음 예시 (화요일)               
