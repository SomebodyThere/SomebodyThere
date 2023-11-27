

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

![자율주행 시내버스의 정차 시스템 개발 erd 다이어그램](https://raw.githubusercontent.com/SomebodyThere/SomebodyThere/main/erd.png)
![자율주행 시내버스의 정차 시스템 개발 erd 다이어그램]()


</br>
</br>

## 📚 UserFlow
||||
|:---:|:---:|
|**비로그인 유저**|**일반회원(로그인 유저)**|
|<>|<>|
</br>

## ✨ 서비스 구현
### 회원(User)
- Create : 일반회원 회원가입, 로그인 및 로그아웃 기능
- Read : 회원 마이페이지 조회(회원정보, 버스노선에 대한 정보)
- Update : 회원 마이페이지 수정(닉네임,소개,우리동네 설정 등) 기능
- Delete : 회원 탈퇴 기능

### 버스 노선(bus line)
- Read : 현재 버스 위치 기능, 버스 번호 조회 기능, 버스 시간 조회 기능, 버스 노선 조회 기능

</br>

## 🖥️ 서비스 화면


### 메인 화면

||||
|:---:|:---:|:---:|
|**비회원 메인 화면**|**현재 버스 위치 조회**|**버스 노선 조회**|

<br/>

### 회원

||||
|:---:|:---:|:---:|
|**회원가입,로그인**|**소셜 로그인**|**마이페이지**|

<br/>

### 버스

||||
|:---:|:---:|:---:|
|**버스 검색**|**버스 노선 검색**|**버스 시간 검색**|


<br/>
