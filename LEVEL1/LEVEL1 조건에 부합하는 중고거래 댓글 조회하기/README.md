### SQL문
SELECT     
A.TITLE,   
A.BOARD_ID,    
B.REPLY_ID,    
B.WRITER_ID,   
B.CONTENTS,   
TO_CHAR(B.CREATED_DATE,'YYYY-MM-DD') AS CREATED_DATE   
FROM USED_GOODS_BOARD A, USED_GOODS_REPLY B   
WHERE A.BOARD_ID = B.BOARD_ID   
    AND TO_CHAR(A.CREATED_DATE,'YYYY-MM') = '2022-10'   
ORDER BY B.CREATED_DATE ASC, A.TITLE ASC  
;  

### 문제  
USED_GOODS_BOARD와 USED_GOODS_REPLY 테이블에서 2022년 10월에 작성된   
게시글 제목, 게시글 ID, 댓글 ID, 댓글 작성자 ID, 댓글 내용, 댓글 작성일을 조회하는 SQL문을 작성해주세요.   
결과는 댓글 작성일을 기준으로 오름차순 정렬해주시고, 댓글 작성일이 같다면 게시글 제목을 기준으로 오름차순 정렬해주세요.  

### 결과
![image1](https://user-images.githubusercontent.com/123911778/261910007-0677c426-da40-486d-a22d-06600299adad.PNG)

### 설명
2개의 Table에서 데이터를 가져올 때는 테이블 명에 별칭을 붙여서 사용한다.
여기서는 USED_GOODS_BOARD 테이블에 A, USED_GOODS_REPLY 테이블에 B라는 별칭을 붙였다.
조건문을 나타내는 WHERE에서 A와 B에서 동시에 가지고 있는 Column인 Board_id가 서로 같다고 명시해주었고
SELECT에서는 어떤 테이블의 Column을 가져 왔는지 A.TITLE, B.REPLY_ID 등의 방식으로 명시한다.
A.CREATED_DATE에는 DATE 자료형이 저장되어 있는데 2022년 10월의 데이터를 가져오기 위해서
TO_CHAR을 사용하여 DATE 자료형을 CHAR 자료형으로 변환하였고 앞의 연도와 달까지만 가져와서 '2022-10'과 비교했다.
ORDER BY은 정렬을 하는 구문으로 먼저 B.CREATED_DATE에 대해 오름차순으로 정렬하고 같은 값이 있을 경우  
A.TITLE에 대해 오름차순으로 정렬한다.
