
<section align="end" style="color: #fff;">
  <p>${\small\texttt{\color{#a9a9a9} last 23.04.11}}$</p>
</section>

<section align="center">

<a href="https://www.pintogether.co.kr" >
<img src="https://github.com/PinTogether/.github/assets/89989211/205a7826-36d3-421f-95a2-d09bb9864d9b" alt="pintogether-logo-horizontal" width="300"/>
</a>

</section>

<br/>
<br/>
<br/>

<section>
   <h2> 목차 </h2>
  
  1. [소개](#-소개-Introduction) 
  2. [프로젝트 진행 기간](#-프로젝트-진행-기간)
  3. [제공하는 기능](#-제공하는-기능)
  4. [팀원 소개](#-팀원-소개)
  5. [서비스 화면](#-서비스-화면)
  6. [사용 기술](#-사용-기술)
  7. [아키텍쳐](#-아키텍쳐-Architecture)
  8. [API](#-API)
  9. [ERD](#-ERD)
  
</section>
<br/>

<section>

  ## 📌 소개 Introduction

  >  [pintogether.co.kr](https://www.pintogether.co.kr) <br/>
  >  좋아하는 장소에 핀을 찍고, 컬렉션을 만들어 친구들과 공유해보세요!  <br/>
  
  <br/>
  Pintogether는 지도를 기반으로 한 장소 공유 웹 서비스 프로젝트입니다.  <br/>
  <br/>

  타인이 알고있는 맛집과 장소들을 한눈에 확인하고 손쉽게 탐색하기 어렵다는 일상의 불편함에서 출발했습니다. <br/>
  이를 해소하기 위해 웹 기반의 장소 목록 서비스를 구상하게 되었습니다. <br/>
  사용자들이 맛집리스트를 발견하고 공유하는 즐거움을 쉽고 편리하게 누릴수 있는 서비스를 추구합니다. <br/>
  
  <br/>

  <h2>📌 프로젝트 진행 기간</h2>

  설계 및 주요 기능 구현 : 24.01.15 ~ 03.31

  실제 서비스 배포를 위한 리펙토링 : 24.04.01 ~ 개발중

  <br/>


  <h2>📌 제공하는 기능</h2>

  * 소셜로그인
  * 장소 검색
    * 현재 LOCALDATA(지방행정 인허가 데이터 개방)에서 가져온 음식점 데이터 약 25만건을 기반으로, 장소 검색기능을 제공하고 있습니다.
    * 장소 검색 기록 조회
  * 지도
  * 프로필 조회, 수정
    * 유저 팔로우
  * 컬렉션(장소목록)
    * 컬렉션 조회, 수정
    * 컬렉션 좋아요, 스크랩
  * 핀(장소저장)
    * 핀 조회, 수정
    * 핀 좋아요
  * 장소 찜
    * 찜한 장소 컬렉션에 핀으로 저장
  * 알림
  * 신고
  * 인기 컬렉션 추천
  * 컬렉션 공유


</section>

<br/>


<section >
  <h2>📌 팀원 소개</h2>
  <table align=center>
    <thead>
      <tr>
          <td align=center width="500">😶</td>
          <td align=center width="500">😎</td>
          <td align=center width="500">😶</td>
          <td align=center width="500">🥰</td>
      </tr>
    </thead>
      <tr>
          <td align=center><a href="https://github.com/jwo1024">이지우(팀장)</a></td> 
          <td align=center><a href="https://github.com/UMGGG">전재영</a></td>
          <td align=center><a href="https://github.com/tehyoyee">김태형</a></td>
          <td align=center><a href="https://github.com/spew11">이은지</a></td>
      </tr>
      <tr>
          <td align=center>프론트엔드, 기획, 디자인</td>
          <td align=center>프론트엔드</td>
          <td align=center>백엔드, 인프라(클라우드), CI/CD</td>
          <td align=center>백엔드, 인프라(클라우드)</td>
      </tr>
      <tr>
          <td align=center>
            - 프로필, 컬렉션, 핀 조회 및 수정 페이지, API연결 <br/>
            - 로그인, 검색, 장소, 알림, 신고 페이지, API연결 <br/>
            - 재사용 가능한 컴포넌트 구현<br/> 
            (컬렉션, 핀, 장소 카드) <br/> 
            (input, textarea, 카드슬라이더) <br/>
            - Redux 활용 로그인 상태관리 <br/>
            - Presigned-url 활용 이미지 업로드 <br/>
            - 활용 가능한 api 및 데이터 서치 <br/>
          </td>
          <td align=center>
            - 네이버 지도, 외부 api 적용 <br/>
            - 지도 이용하는 기능 구현 <br/>
            - 페이지 기본 레이아웃, 사이드바, 지도 오버레이 구현 <br/>
            - 각 페이지와 지도 연동 <br/>
            - 메인페이지, 프로필, 설정, 컬렉션 생성 페이지 담당 <br/>
            - 스켈레톤 ui <br/>
          </td>
          <td align=center>
            - ERD/API<br/>
            - 로그인 (JWT, OAuth(google, kakao, naver)<br/>
            - 검색엔진<br/>
            - 지도 데이터 관리<br/>
            - Elastic Stack (ING)<br/>
            - CI/CD 깃헙액션<br/>
            - Github Submodule <br/>
            - AWS (Amplify, ElasticBeanstalk, RDS, S3, ACM, IAM, Route53...)<br/>
          </td>
          <td align=center>
            - DB설계 및 엔티티 매핑<br/>
            - API설계 <br/>
            - 멤버, 컬렉션, 알림, 검색 API 구현 <br/>
            - web socket 기반 알림 구현 <br/>
          </td>
      </tr>
  </table>
</section>
<br/>

<section>
  <h2>📌 서비스 화면</h2>
  
  [프레젠테이션으로 보기](https://www.canva.com/design/DAGB4VnAkAw/npGrZzdtfy3Z-uApnkKp_A/view?utm_content=DAGB4VnAkAw&utm_campaign=designshare&utm_medium=link&utm_source=editor)
  
![2](https://github.com/PinTogether/.github/assets/89989211/64870e27-121e-4903-8720-d0677b28108a)
![3](https://github.com/PinTogether/.github/assets/89989211/952921a3-2c31-434f-aec7-fa16bd25b4eb)
![4](https://github.com/PinTogether/.github/assets/89989211/3252cbf0-fa8e-40e9-a6c6-ed5f8892c2b8)
![5](https://github.com/PinTogether/.github/assets/89989211/7579e7c7-e902-408a-afe8-9c14faf28394)
![6](https://github.com/PinTogether/.github/assets/89989211/e5a0eae6-76d1-4e61-bb3e-9a9b63e316da)
![7](https://github.com/PinTogether/.github/assets/89989211/22043465-fde2-4600-96ba-31dfeb4fa69a)
![8](https://github.com/PinTogether/.github/assets/89989211/1cae364b-0cfd-4add-8672-8ea2c7a983b1)
![9](https://github.com/PinTogether/.github/assets/89989211/4c827fa3-1ef9-414e-80d3-4c8e966c6763)
![10](https://github.com/PinTogether/.github/assets/89989211/76e2797d-c926-45e5-b278-3a245351ff23)
![11](https://github.com/PinTogether/.github/assets/89989211/8127abc4-d278-418b-b8eb-96481bc29350)
![12](https://github.com/PinTogether/.github/assets/89989211/fdd24d6c-63f7-4a99-920d-7dabe235c81d)
![13](https://github.com/PinTogether/.github/assets/89989211/b679347b-dd0e-49ea-8899-b06421126c39)
![14](https://github.com/PinTogether/.github/assets/89989211/668bb1da-f623-4d1b-9c0f-6f900c6334f8)
![15](https://github.com/PinTogether/.github/assets/89989211/d6e76bad-5957-4713-9fac-ce3a92a34382)
![16](https://github.com/PinTogether/.github/assets/89989211/7462d2b7-09c2-4700-9d3d-7f5144aa4768)


<section>
  <h2>📌 사용 기술</h2>

  ### Backend
  * Java 17
  * Spring Boot 3.2.2
  * Spring Security(OAuth2)
  * Spring Data JPA (Jpa Auditing, 
  * Spring Cloud-aws 2.2.6
  * Spring Websocket
  * Gradle 8.5
  * Slf4j
  * Jwt

  ### Frontend
  * HTML5/CSS3
  * React 18
  * Typescript 5.0
  * Next.js 14.1.0
  * Redux 5.0.1
  * Redux Toolkit
  * SCSS 0.2.4
  * ESLint

  ### DB
  * MariaDB 10.11.6
  * Elastic Stack(Beats, Logstash, ElasticSearch, Kibana) 접목중

  ### Open API
  * [Naver Cloud Maps(Web Dynamic Map)](https://www.ncloud.com/product/applicationService/maps)
  * [SGIS Geocode](https://sgis.kostat.go.kr/view/index)
  * [GeoLocation](https://w3c.github.io/geolocation-api/#geolocation_interface)

  ### 데이터
  * [LOCALDATA(지방행정 인허가 데이터 개방)](https://www.localdata.go.kr/main.do)

  ### AWS
  * Elastic Beanstalk(EC2, Application LoadBalencer, CloudWatch)
  * Amplify
  * S3(presgined-url)
  * Route53
  * RDS
  * ACM

  ### CI/CD
  * Github Action
  * Git Submodule

  ### 도구
  * VScode
  * IntelliJ IDEA
  * MySQLWorkbench
  * Postman
  * Vercel (프론트 페이지 테스트 용도)

  ### 협업
  * Notion
  * Slack

  ### 디자인
  * Figma

</section>


<section>
  <h2>📌 아키텍쳐 Architecture</h2>
  <img src="https://github.com/PinTogether/.github/assets/89989211/dc58d944-f6ea-498b-908d-5f9dff6834ce" alt="pintogether-architecture" width="800"/>

  <h2>📌 Api</h2>
  
  * [API Notion Link](https://wellcome-jiwoo-land.notion.site/API-a93bfddcca4941289848dc44c077f107?pvs=4)
  <img src="https://github.com/PinTogether/.github/assets/95565246/0a07c184-5323-44a2-95c1-11b0f81548c6" alt="pintogether-api" />

  <h2>📌 ERD</h2>
  <img src="https://github.com/PinTogether/.github/assets/95565246/f84a0533-1f3b-4d17-a2ec-6c2c8af6631e" alt="pintogether-erd" />

</section>



