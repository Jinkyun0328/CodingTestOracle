### SQL문
![image1](https://user-images.githubusercontent.com/123911778/263866781-a1e8c5b0-caf4-4081-9955-432190ae19e8.PNG)

### 문제  
![image2](https://user-images.githubusercontent.com/123911778/263866785-ea874046-643f-488d-9755-643c1c9e1843.PNG)

### 결과
![image3](https://user-images.githubusercontent.com/123911778/263866778-8cf84373-22f0-4390-9d06-85639b342640.PNG)

### 설명
MEMBER_PROFILE 테이블과 REST_REVIEW 테이블을 INNER JOIN한다.           
리뷰를 남긴 개수가 최대 개수와 같은 멤버를 찾아 데이터를 조회한다.           

COUNT 함수를 사용하여 리뷰를 남긴 횟수를 센 다음 내림차순으로 정렬하여 첫 번째 행만 가져옴으로 최댓값을 구한다.           
최댓값을 가지는 MEMBER_ID만을 조회하여 이름, 리뷰, 리뷰날짜를 출력한다.               
