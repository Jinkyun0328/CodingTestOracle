### SQL문
![image1](https://user-images.githubusercontent.com/123911778/263133553-639cd0f6-0396-4017-9f20-7f3ff414e518.PNG)

### 문제  
![image2](https://user-images.githubusercontent.com/123911778/263133558-d2a7d400-de01-43d8-9688-0782a4a62e05.PNG)

### 결과
![image3](https://user-images.githubusercontent.com/123911778/263133562-ac0a8827-4f92-4dde-b7c0-96053b945bb7.PNG)

### 설명
입양을 간 동물 중, 보호 기간이 가장 길었던 동물 두 마리의 정보를 조회하려고 한다.
오라클에서는 날짜형 사이의 차를 구할 때는 빼기 연산을 사용하여 구할 수 있다.

INS 테이블과 OUTS 테이블에서 데이터를 모두 가져오므로 INNER JOIN을 사용하여 연결하였고
INNER JOIN을 한 상태에서는 INS와 OUTS에 등록되어 있는 ID만 출력되므로
JOIN한 테이블에는 모두 입양을 간 동물만 들어있다.

OUTS의 DATE와 INTS의 DATE의 차를 사용하여 정렬한 다음
ROWNUM을 사용하여 위에서부터 2개의 행만 출력했다.

서브쿼리를 사용하여 FROM 절에 쿼리를 만든 이유는 FROM 내부에 있는 WHERE에 ROWNUM을 사용하면
정렬을 하기 전에 튜플을 구분하기 때문에 정렬되지 않은 상태에서 위에서부터 2개의 튜블을 출력하기 때문이다.
