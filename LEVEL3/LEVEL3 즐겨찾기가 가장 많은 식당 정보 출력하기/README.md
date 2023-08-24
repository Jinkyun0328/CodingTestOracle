### SQL문
![image1](https://user-images.githubusercontent.com/123911778/262871150-fe6af2ed-84ca-4113-93ab-bce79f5e733e.PNG)

### 문제  
![image2](https://user-images.githubusercontent.com/123911778/262871153-685b4a92-a9f5-42f5-93ed-71c7446af2e7.PNG)

### 결과
![image3](https://user-images.githubusercontent.com/123911778/262871154-baa123b0-0ae6-46ad-a6c5-8d6112782768.PNG)

### 설명         
음식종류별로 즐겨찾기수가 가장 많은 식당을 찾는 것이므로 FOOD_TYPE을 그룹화하여 MAX(FAVERITES)을 집계한다.
출력하는 것이 음식 종류, ID, 식당 이름, 즐겨찾기수이므로 한 번에 출력하기는 어렵다.         
FROM절에서 이중쿼리를 사용하여 FOOD_TYPE과 MAX(FAVORITES)의 테이블을 만들어 조회하였고         
FOOD_TYPE을 같게 설정하여 INNER JOIN했다.         
즐겨찾기의 최댓값인 식당이 필요한 것이므로 WHERE에서 즐겨찾기가 최댓값과 같은 것을 조건식으로 작성했다.           
