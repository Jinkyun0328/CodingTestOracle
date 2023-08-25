### SQL문
![image1](https://user-images.githubusercontent.com/123911778/263134173-50effc65-c530-49e4-a1a0-0d3b31a44853.PNG)

### 문제  
![image2](https://user-images.githubusercontent.com/123911778/263134175-96950054-0b45-4bd3-9a6d-f434e9416ac5.PNG)

### 결과
![image3](https://user-images.githubusercontent.com/123911778/263134176-8fcb0694-9ee5-4d15-9548-dc0bc96ddb50.PNG)

### 설명
아직 입양을 못 간 동물의 데이터를 조회하므로 INS 테이블에는있으나 OUTS 테이블에는 없는 ID를 조회해야 한다.                  
INS 테이블이 주가 되므로 LEFT JOIN을 사용하여 JOIN하고 OUTS의 DATETIME에 NULL이 저장되어 있는 튜플을 찾았다.                  
이전에는 ROWNUM을 사용하여 WHERE절에서 상위 2개의 행을 출력했는데                  
이번에는 FETCH NEXT 3 ROWS ONLY를 사용하여 위에서부터 3개의 행을 출력했다.                  
이 방식은 WHERE절에 포함되어 있는 것이 아니기 때문에 정렬이 모두 된 상태에서 위에서부터 3개의 행을 출력한다.                  
