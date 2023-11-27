

## 👩🏻‍💻 팀원 소개  

|박한백|김정훈|윤희정|이상기|
|:---:|:---:|:---:|:---:|
|<img alt="박한백" src="https://user-images.githubusercontent.com/80394894/215561204-8e085531-f851-48d4-bb3e-e8aad142565a.png" height="120" width="120">|<img alt="김정훈" src="https://user-images.githubusercontent.com/80394894/215561204-8e085531-f851-48d4-bb3e-e8aad142565a.png" height="120" width="120">|<img alt="윤희정" src="https://user-images.githubusercontent.com/80394894/215561134-da53fca5-b85c-4d2f-b077-e83a707f3de0.png" height="120" width="120">|<img alt="이상기" src="https://user-images.githubusercontent.com/80394894/215555107-23fa07fe-fe13-4fe2-8c2f-572ba9f3917c.png" height="120" width="120">|
|**FE**|**FE**|**FE**|**BE**|*FE**|

## 🚌 서비스 소개
- 자율주행 시내버스가 곧 등장할 것으로 예상합니다.
- 시내버스는 주행 경로가 미리 지정되어 있어 자율주행의 안전성을 비교적 쉽게 높일 수 있기 때문입니다.
- 자율주행 시내버스가 등장하면 정류장에 정차하기 위한 적절한 시스템이 필요합니다.
- 최적의 시내버스 운행 방안을 찾기 위해 프로젝트를 시작하게 되었습니다.
</br>

## 🚏 자율주행 시내버스의 정차 시스템 개발 목표
- 앱과 웹은 승객이 사용하게 되고 승객들은 앱 혹은 웹을 통해 서버에 탑승 요청을 보낼 수 있고 서버는 이를 확인하고 저장합니다.
- 버스 시스템은 우선 차량 내부 승객들의 하차 여부를 확인하고 차량에 탑승하고 있는 승객 중 하차 의사가 있는 승객이 있다면 정차 시스템과 상관없이 정류장에 정차하게 됩니다.
- 만약 탑승 중인 승객들이 하차 의사가 없다면, 정차 시스템이 작동되고 자율주행 버스가 정류장에 가까워 지면 정류장 도착 전에 서버에 도착할 정류장에서 해당 버스에 탑승할 인원이 있는지 확인합니다.
- 탑승할 승객이 있다면 자율주행 버스는 도착할 정류장을 이미지 인식하기 시작합니다.
- 해당 정류장에 사람이 있는지 판단하고 여기서 사람이 있다면 정차하게 되고, 사람이 없다면 정차하지 않고 계속 주행하게 됩니다.
- 자율주행 버스 정차 시스템은 버스의 정차 여부를 승객의 요청, 카메라를 통한 이미지 인식 두 가지를 통해 이중으로 판단하게 됩니다. 
</br>



## 🗓️ 프로젝트 기간
- 2023.09.01 ~ 2023.12.14
</br>

## 🔗 배포 링크
-  
</br>

## 📌 기술 스택 및 아키텍처



</br>
</br>

## 📓 ERD

![자율주행 시내버스의 정차 시스템 개발 erd 다이어그램](https://user-images.githubusercontent.com/80394894/215329542-fdfa3b2e-a627-4427-a68f-9cc50e2274dc.PNG)

</br>
</br>

## 📚 UserFlow
||||
|:---:|:---:|:---:|
|**비로그인 유저**|**일반회원(로그인 유저)**|**퍼포머(로그인 유저)**|
|<img width="1888" alt="userflow-User" src="https://user-images.githubusercontent.com/80394894/215343144-0cbd0ed3-e980-43b7-ad21-e0a4844a8794.png">|<img width="2224" alt="userflow-Member" src="https://user-images.githubusercontent.com/80394894/215343162-e947cca2-b63a-4fd4-987e-98976c6b2fb1.png">|<img width="2240" alt="userflow-Performer" src="https://user-images.githubusercontent.com/80394894/215343177-c9ce7969-88f3-47e1-b65f-f35cc09dedae.png">|
</br>

## ✨ 서비스 구현
### 회원(User, Performer)
- Create : 일반회원 또는 퍼포머회원으로 회원가입, 로그인 및 로그아웃 기능
- Read : 회원 마이페이지 조회(회원정보, 공연예약에 대한 정보), 다른 회원의 프로필 조회 기능
- Update : 회원 마이페이지 수정(닉네임,소개,우리동네 설정 등) 기능
- Delete : 회원 탈퇴 기능

### 게시글(Article)
- Create : 일반 회원/퍼포머 게시글 및 댓글 작성 기능
- Read : 비회원/일반 회원/퍼포머 게시글 조회 및 게시글 검색 기능
- Update : 일반 회원/퍼포머 게시글 및 댓글 수정 기능
- Delete : 일반 회원/퍼포머 게시글 및 댓글 삭제 가능

### 공연(Show)
- Create : 퍼포머 공연 작성 기능, 일반 회원은 리뷰 작성 기능, 퍼포머/일반 회원 공연 예약 생성 기능
- Read : 퍼포머/일반 회원/비회원 공연 조회 가능, 일반 회원/비회원 답변 조회 기능, 퍼포머 판매 공연 조회 기능, 일반 회원 공연 예약 조회 기능
- Update : 퍼포머 공연 수정 기능, 일반 회원 답변 수정 기능
- Delete : 퍼포머 공연 삭제 기능, 회원 답변 삭제 기능

</br>

## 🖥️ 서비스 화면


### 메인 화면

||||
|:---:|:---:|:---:|
|**비회원 메인 화면**|**지역별 날짜별 공연 조회**|**회원 지역별 현황 조회**|
|<img width="100%" src="https://user-images.githubusercontent.com/95069395/215596135-f333470c-990c-4641-bfdf-7c32958874e4.gif"/>|<img width="100%" src="https://user-images.githubusercontent.com/95069395/215596154-99f4d010-c452-4380-8dd5-c33b1e54fedb.gif"/>|<img width="100%" src="https://user-images.githubusercontent.com/95069395/215596163-560a30d3-5aea-4ca6-a091-7480a2b10ed4.gif"/>|
|**메인 공연 검색**|**인기 게시글**|
|<img width="100%" src="https://user-images.githubusercontent.com/95069395/215596163-560a30d3-5aea-4ca6-a091-7480a2b10ed4.gif"/>|<img width="100%" src="https://user-images.githubusercontent.com/95069395/215596148-77b7c68d-35d5-4a1a-b93b-90697fb04c0a.gif"/>||

<br/>

### 회원

||||
|:---:|:---:|:---:|
|**회원가입,로그인**|**소셜 로그인**|**마이페이지**|
|<img width="100%" src="https://user-images.githubusercontent.com/95069395/215601508-d20fd052-7c1a-479c-bf5c-399457785c9c.gif"/>|<img width="100%" src="https://user-images.githubusercontent.com/95069395/215601501-c6726d15-931b-47db-981c-a6bf76704c1d.gif"/>|<img width="100%" src="https://user-images.githubusercontent.com/95069395/215601490-146290d6-2e9d-403b-b44e-e594de485ac5.gif"/>|

<br/>

### 공연

||||
|:---:|:---:|:---:|
|**공연 검색**|**공연 댓글**|**공연 예약**|
|<img width="100%" src="https://user-images.githubusercontent.com/95069395/216259136-a2b9c592-75ff-4299-b07d-b3e86a6731ba.gif"/>|<img width="100%" src="https://user-images.githubusercontent.com/95069395/216258213-88666074-201a-4240-b110-6d7fbf117096.gif"/>|<img width="100%" src="https://user-images.githubusercontent.com/95069395/216258226-cdd582a8-ad1f-403a-98ce-a1740fdbd174.gif"/>|
|**공연 **|**공연 지도조회**||
|<img width="100%" src=""/>|<img width="100%" src=""/>||

<br/>


### 커뮤니티(게시글)

||||
|:---:|:---:|:---:|
|**게시글 작성**|**게시글 수정**|**게시글 조회 및 검색**|
|<img width="100%" src="https://user-images.githubusercontent.com/95069395/215602632-169dd28b-08b4-476d-b25e-9ee7ef2f70d3.gif"/>|<img width="100%" src="https://user-images.githubusercontent.com/95069395/215602652-84c6e0ef-ac00-42e9-b992-b4b43cb7e28b.gif"/>|<img width="100%" src="https://user-images.githubusercontent.com/95069395/215605338-53b03d4b-7298-43e9-bd0c-c8a37db8df50.gif"/>|
|**게시글 삭제**|**게시글,댓글 좋아요**||
|<img width="100%" src="https://user-images.githubusercontent.com/95069395/215602688-cfd61585-d60b-4744-9a87-882e2e2fffe3.gif"/>|<img width="100%" src="https://user-images.githubusercontent.com/95069395/215602675-43008b57-fda5-4f53-aa6a-8f4829ffc575.gif"/>||

<br/>
