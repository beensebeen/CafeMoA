# CafeMo☕️ 우리동네 카페 추천 프로젝트

```bash
전체 카페의 90%를 차지하지만 정보가 부족한 '동네카페'와 사용자를 연결하는 추천 플랫폼입니다.
<br>카페 점주는 효과적인 홍보 채널을 얻고, 사용자는 자신의 취향에 맞는 새로운 공간을 발견하는 기회를 가집니다.
```

---

## 1️⃣ 프로젝트 개요

### 🚩 기획 배경

프로젝트 팀은 국내 커피 시장의 정보 불균형 문제에서 기회를 발견했습니다.

- **정보의 부재**: 국내 카페의 **90%는 '동네카페'**이지만, 사용자들은 프랜차이즈나 광고를 집행하는 카페 정보만 주로 접하게 됩니다.
- **탐색의 어려움**: 사용자는 매번 가던 곳만 가거나, **자신의 취향에 맞는 새로운 카페를 발견**하는 데 어려움을 겪습니다.
- **홍보의 한계**: 동네카페 점주들은 **마땅한 홍보 수단이 없어** 잠재 고객에게 카페를 알리지 못하고 쉽게 폐업하곤 합니다.

### 🚩 프로젝트 목표

이러한 문제를 해결하기 위해 다음과 같은 솔루션을 구현하고자 합니다.

- **정보 제공의 중심**: 흩어져 있는 **동네카페의 상세 정보(위치, 메뉴, 시간, 분위기 등)를 한곳에 모아** 사용자에게 제공합니다.
- **개인화된 카페 추천**: **리뷰와 사용자 취향 데이터를 기반으로 한 추천 시스템**을 통해 만족도 높은 카페 방문 경험을 유도합니다.
- **상생 플랫폼 구축**: 사용자에게는 **새로운 카페를 탐색하는 즐거움을, 점주에게는 자신의 가게를 알릴 수 있는 기회**를 제공하여 서로에게 도움이 되는 서비스를 만듭니다.

### 🚩 프로젝트 확장성

본 프로젝트는 동서울대학교 인근 카페 정보를 시작으로, 향후 전국 주요 대학가 및 지역 상권으로 서비스를 확대할 계획입니다.

- **서울 및 수도권 지역 확장**
- **카페 운영자 직접 등록 기능**
- **취향 기반 추천 알고리즘 도입**
- **지역 상권 데이터 분석 리포트화**

---

## 2️⃣ 기술 스택 세부 명세

### 🚩 개발 도구

**Android Studio 4.2**

- 선택이유: IntelliJ의 강력한 코드 편집기, 개발자 도구와 안드로이드 앱을 빌드 할 때 생산성을 높여주는 기능을 제공.

### 🚩 서버

**닷홈**

- 도입배경: 안드로이드에서는 데이터베이스와의 직접적인 접속 불가능하여 웹 서버의 중계 필요.
- 해결방안: 무료 호스팅 서비스를 제공하는 호스팅 업체인 닷홈으로 도메인 생성.

**File Zilla**

- 선택이유: 닷홈에서 생성된 도메인을 입력해 서버와 연결되면 디렉터리 조회됨. 홈 디렉토리인 html 폴더에 PHP 파일을 업로드하고, 다운로드할 수 있음.

### 🚩 DB

**phpMyAdmin**

- 효과: 대부분의 MySQL 기능을 지원해서 데이터베이스를 생성하고 관리하는데 간단하고 편리.

### 🚩 API

**Kakao 지도 API**

- 목적: 카카오 지도 위에 사용자의 현재 위치와 특정 장소들을 마커 표시하고, 라인을 표시해 경로 좌표 데이터를 이용 가능.

---

## 2️⃣ 개발 일정

### 🚩 WBS (Work Breakdown Structure)

<img width="545" height="284" alt="Image" src="https://github.com/user-attachments/assets/53e452aa-6761-4c14-9f68-b6e6b4242d08" />

### 🚩 간트 차트(Gantt Chart)

개발 기간: 2022.03 ~ 2022.11 (총 9개월)
3월은 팀원 및 프로젝트 아이디어 선정 기간이며, 아래 사진은 4월부터 11월에 대한 일정
<img width="579" height="370" alt="Image" src="https://github.com/user-attachments/assets/3d3470ec-dad2-436c-97bf-1608a808b93e" />

---

## 3️⃣ 산출물

### 🚩 ERD

<img width="658" height="292" alt="Image" src="https://github.com/user-attachments/assets/c3b401e7-c879-4965-aaa7-3ed939042712" />

## 4️⃣ 주요 기능

### 🚩 로그인 기능

<img width="316" height="362" alt="Image" src="https://github.com/user-attachments/assets/e9f439f1-9ea8-4b17-bc61-a9aa5f24d2ef" />
<img width="301" height="402" alt="Image" src="https://github.com/user-attachments/assets/2b608dab-4c9e-4d7c-8fda-a131d0d7278b" />
<img width="579" height="310" alt="Image" src="https://github.com/user-attachments/assets/ec74d533-100f-4fbb-879f-3fb84890d8d3" />
<img width="592" height="541" alt="Image" src="https://github.com/user-attachments/assets/b865f135-446e-4157-a032-6628fcccaab3" /></br>
회원가입, 로그인, 계정찾기, 로그아웃, 회원정보수정, 탈퇴 가능.

### 🚩 위치제공 기능

<img width="310" height="571" alt="Image" src="https://github.com/user-attachments/assets/465b6833-5604-48d3-9489-d2befc451bf8" />
<img width="588" height="403" alt="Image" src="https://github.com/user-attachments/assets/f7cfca58-ef06-49d3-a4eb-80ffd8198fc0" /></br>

사용자의 현재 위치를 받아 주변의 위치한 카페를 마커로 맵에 표시.

### 🚩 카페정보 기능

## <img width="296" height="392" alt="Image" src="https://github.com/user-attachments/assets/9aac346f-5cb9-44ca-b575-f78d3a66e44c" /></br>

- 사용자는 카페를 선택하여 해당 카페에 대한 정보(이름, 번호, 영업/휴무일, 주소 등)를 얻을 수 있음.
- 카페에 있는 번호로 전화 걸기 가능.
- 목적지로 가는 길을 제공하는 카카오맵 웹/앱으로 이동.

### 🚩 리뷰 기능

<img width="290" height="229" alt="Image" src="https://github.com/user-attachments/assets/50596b00-0a35-4747-9f6e-13b4ae9eeee0" /></br>

- 리뷰 작성/관리 뿐만 아니라, 다른 사용자가 작성한 리뷰 확인 가능.

### 🚩 북마크 기능

<img width="289" height="571" alt="Image" src="https://github.com/user-attachments/assets/f30fc40d-d91e-410e-aee3-8fc9f47e5e29" /></br>

- 마음에 드는 카페를 북마크하여 저장할 수 있음.
- 북마크 삭제 버튼 클릭 시 다이얼로그 메시지가 출력되며 해당 카페의 북마크가 삭제됨.

### 📌 프로젝트에서 사용된 주요 기술 스택

### 💻 Backend

- <img src="https://img.shields.io/badge/java-007396?style=flat-square&logo=java&logoColor=white"/>
- <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black"/>
- <img src="https://img.shields.io/badge/JSON-000000?style=flat-square&logo=json&logoColor=white"/>
- <img src="https://img.shields.io/badge/PHP-777BB4?style=flat-square&logo=php&logoColor=white"/>

### 🎨 Main Tool

- <img src="https://img.shields.io/badge/Android Studio-3DDC84?style=flat-square&logo=Android Studio&logoColor=white"/>

### 🗄 Database

- <img src="https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=MySQL&logoColor=white"/>

### 🛠 협업 툴

- <img src="https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white"/>
