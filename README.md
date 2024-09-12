# 💪 Pocket-Health - 헬스 프로젝트
![이미지](https://www.ftimes.kr/news/photo/202110/13278_14865_1142.jpg)
# 📃 목차
- [Pocket-Health Web Page v2.0](#pocket-health-web-page-v2.0)
- [배포주소](#배포주소)
- [프로젝트 소개](#프로젝트-소개)
- [시작 가이드](#시작-가이드)
- [Stacks](#stacks)
- [프로젝트 파일 구조](#프로젝트-파일-구조)
- [주요 기능 목록](#주요-기능-목록)
- [페이지별 서비스 화면](#페이지별-서비스-화면)
- [트러블 슈팅](#트러블-슈팅)
- [버전 업](#버전-업)

# 💉 Pocket-Health Web Page v2.0
> 전체 개발 기간 : 2024-07-01 ~ 2024-10-01<br>
> UI 구현 : 2024-07-01 ~ 2024-7-20<br>
> 기능 구현 : 2024-08-01 ~ 2024-10-01<br>

## 📦 배포주소
> 개발 버전 : [Pocket-Health](https://ohmycode-readme.netlify.app/)<br>
> 프론트 서버 : [front](https://ohmycode-readme.netlify.app/)<br>
> 백엔드 서버 : [backend](https://ohmycode-readme.netlify.app/)<br>

## 📖 프로젝트 소개 
> Pocket-Health는 헬스를 하는데 동기부여를 줘서 원하는 목표를 달성할 수 있도록 만든 프로젝트 입니다.<br>
> 운동을 게임처럼 느끼게 함으로써 재미와 장기적인 운동 습관을 만들 수 있습니다.<br>
> 운동을 전문적으로 하는 분들에게 피드백을 받을 수 있습니다.<br>
> 자신의 관종끼를 자랑할 수 있습니다.<br>

## ✨ 시작 가이드

### 🎉 Requirements
For building and running the application you need:

- [Node.js 14.19.3](https://nodejs.org/ca/blog/release/v14.19.3/)
- [Npm 9.2.0](https://www.npmjs.com/package/npm/v/9.2.0)
- [Strapi 3.6.6](https://www.npmjs.com/package/strapi/v/3.6.6)
### 🎉 Installation
```
$ git clone https://github.com/Voluntain-SKKU/Voluntain-2nd.git
$ cd Voluntain-2nd
```
### 🎉 Backend
```
$ cd strapi-backend
$ nvm use v.14.19.3
$ npm install
$ npm run develop
```
### 🎉 FrontEnd
```
$ cd voluntain-app
$ nvm use v.14.19.3
$ npm install 
$ npm run dev
```

## 🛠 Stacks
### 🔧 Environment
<div>
  <img src="https://img.shields.io/badge/Visual Studio Code-007ACC?style=flat-square&logo=Visual Studio Code&logoColor=white"/>
  <img src="https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white"/>
  <img src="https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=GitHub&logoColor=white"/>
</div>

### 🔧 Congin
![NPM](https://img.shields.io/badge/NPM-%23CB3837.svg?style=for-the-badge&logo=npm&logoColor=white)

### 🔧 Development
<div>
<img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black"/>
<img src="https://img.shields.io/badge/Tailwind CSS-06B6D4?style=flat-square&logo=Tailwind CSS&logoColor=white"/>
<img src="https://img.shields.io/badge/Typescript-3178C6?style=flat-square&logo=Typescript&logoColor=white"/>
<img src="https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=React&logoColor=black"/>
<img src="https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=Next.js&logoColor=white"/>
<img src="https://img.shields.io/badge/Express-000000?style=flat-square&logo=Express&logoColor=white"/>
<img src="https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=Node.js&logoColor=white"/>
</div>

### 🔧 Communication
![Notion](https://img.shields.io/badge/Notion-%23000000.svg?style=for-the-badge&logo=notion&logoColor=white)
![Google Meet](https://img.shields.io/badge/Google%20Meet-00897B?style=for-the-badge&logo=google-meet&logoColor=white)
![Slack](https://img.shields.io/badge/Slack-4A154B?style=for-the-badge&logo=slack&logoColor=white)

### 🔧 Design
![Figma Badge](https://img.shields.io/badge/Figma-pink?style=for-the-badge&logo=figma&logoColor=white)

## 📁 프로젝트 파일 구조
```
├── README.md
├── package-lock.json
├── package.json
├── strapi-backend : 
│   ├── README.md
│   ├── api : db model, api 관련 정보 폴더
│   │   ├── about
│   │   ├── course
│   │   └── lecture
│   ├── config : 서버, 데이터베이스 관련 정보 폴더
│   │   ├── database.js
│   │   ├── env : 배포 환경(NODE_ENV = production) 일 때 설정 정보 폴더
│   │   ├── functions : 프로젝트에서 실행되는 함수 관련 정보 폴더
│   │   └── server.js
│   ├── extensions
│   │   └── users-permissions : 권한 정보
│   ├── favicon.ico
│   ├── package-lock.json
│   ├── package.json
│   └── public
│       ├── robots.txt
│       └── uploads : 강의 별 사진
└── voluntain-app : 프론트엔드
    ├── README.md
    ├── components
    │   ├── CourseCard.js
    │   ├── Footer.js
    │   ├── LectureCards.js
    │   ├── MainBanner.js : 메인 페이지에 있는 남색 배너 컴포넌트, 커뮤니티 이름과 슬로건을 포함.
    │   ├── MainCard.js
    │   ├── MainCookieCard.js
    │   ├── NavigationBar.js : 네비게이션 바 컴포넌트, _app.js에서 공통으로 전체 페이지에 포함됨.
    │   ├── RecentLecture.js
    │   └── useWindowSize.js
    ├── config
    │   └── next.config.js
    ├── lib
    │   ├── context.js
    │   └── ga
    ├── next.config.js
    ├── package-lock.json
    ├── package.json
    ├── pages
    │   ├── _app.js
    │   ├── _document.js
    │   ├── about.js
    │   ├── course
    │   ├── index.js
    │   ├── lecture
    │   ├── newcourse
    │   ├── question.js
    │   └── setting.js
    ├── public
    │   ├── favicon.ico
    │   └── logo_about.png
    └── styles
        └── Home.module.css
```

## 🎁 주요 기능 목록
### ⭐️ 강좌 선택 및 강의 영상 시청 기능
Scratch, Python 2개 강좌 및 각 강좌마다 10개 가량의 강의 영상 제공
추후 지속적으로 강좌 추가 및 업로드 예정
### ⭐️ 강의 관련 및 단체에 대한 자유로운 댓글 작성 가능
Disqus를 이용하여 강의 관련 질문이나 단체에 대한 질문 작성 가능
### ⭐️ 이어 학습하기 기능
Cookie 기능을 이용하여 이전에 학습했던 내용 이후부터 바로 학습 가능

## 🖥 페이지별 서비스 화면
### 💡 초기 화면
<img src= "https://raw.githubusercontent.com/wlwlsus/shabit/main/image/gifs/Login3-HQ.gif">

### 💡 회원가입 화면
<img src= "https://raw.githubusercontent.com/wlwlsus/shabit/main/image/gifs/Login3-HQ.gif">

### 💡 로그인 화면
<img src= "https://raw.githubusercontent.com/wlwlsus/shabit/main/image/gifs/Login3-HQ.gif"> 

### 💡 로그아웃 화면
<img src= "https://raw.githubusercontent.com/wlwlsus/shabit/main/image/gifs/Login3-HQ.gif">  

### 💡 메인 화면
<img src= "https://raw.githubusercontent.com/wlwlsus/shabit/main/image/gifs/Login3-HQ.gif">

### 💡 채팅 화면
<img src= "https://raw.githubusercontent.com/wlwlsus/shabit/main/image/gifs/Login3-HQ.gif">

## 💥 트러블 슈팅
- 실시간 채팅시 전송을 주고 받는데 딜레이가 생김
- [탭메뉴 프로필 버튼 이슈](https://github.com/likelion-project-README/README/wiki/README-8.%ED%8A%B8%EB%9F%AC%EB%B8%94-%EC%8A%88%ED%8C%85_%ED%83%AD%EB%A9%94%EB%89%B4-%ED%94%84%EB%A1%9C%ED%95%84-%EB%B2%84%ED%8A%BC-%EC%9D%B4%EC%8A%88)
- [프로필 수정 이슈](https://github.com/likelion-project-README/README/wiki/README-8.%ED%8A%B8%EB%9F%AC%EB%B8%94-%EC%8A%88%ED%8C%85_%ED%94%84%EB%A1%9C%ED%95%84-%EC%88%98%EC%A0%95-%EC%9D%B4%EC%8A%88)

## 📈 버전 업
#### [v1.2] 2024.08.01
* 채팅 기능 추가
* API 모듈화 : API를 불러오는 코드의 반복이 많아 모듈화할 예정
* lighthouse Performance 증진
  - 모든 페이지에서 특히 Best Practices & SEO 점수는 90~100으로 우수
  - Performance 점수가 대체적으로 미흡한 문제
  <img src= "https://user-images.githubusercontent.com/112460466/210591134-09bf8efd-3c34-4b99-a3d7-895ca99e1457.png">
* 23-01-17 성능 개선 내용
  <img src= "https://user-images.githubusercontent.com/106502312/212872369-7ceeb2cf-d551-41d2-bfb0-01e35e9903fe.png"> 
  - 이미지 최적화
    + <img> 요소에 width , height 속성값을 명시해 불필요한 Reflow를 방지했습니다.
    + browser-image-compression 라이브러리를 사용해 유저가 업로드하는 이미지를 압축했습니다.
    + Intersection Observer API를 사용해 Lazy Loading 기법을 적용하여 홈 피드의 게시글 이미지가 viewport 내에 들어오는 순간 로딩되도록 변경했습니다.
  - 웹폰트 최적화
    + WOFF2 포맷을 추가하고 가장 우선적으로 적용되도록 선언했습니다.
    + 서브셋 폰트로 교체해 용량을 줄였습니다.

<div align="right">
  
[목차로](#목차)

</div>
