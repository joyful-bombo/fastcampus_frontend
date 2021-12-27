## 💡 Front-end development
- HTML, CSS, JS를 사용해 데이터를 GUI로 변환하고, 사용자와 상호 작용할 수 있도록 하는 것

### Business Logic
- 웹 사이트가 동작하는데 필요한 핵심 데이터 처리를 수행하는 알고리즘

### 💡 Full-stack development
- Front-end 부터 Back-end 까지 모든 소프트웨어 스택을 개발하는 것

## 💡 Front-end Tech
- HTML (Hyper Text Markup Language) <U>**구조**</U>
  - 페이지의 제목, 문단, 표, 이미지, 동영상 등 <U>**웹의 구조**</U>를 담당.
- CSS (Cascading Style Sheets) <U>**스타일**</U>
  - 실제 화면에 표시되는 방법(색상, 크기, 폰트, 레이아웃 등)을 지정해 콘텐츠를 꾸며주는 <U>**시작적인 표현(정적)**</U>을 담당
- JS(JavaScript) <U>**동적**</U>
  - 콘텐츠를 바꾸고 움직이는 등 페이지를 동작시키는 동적 처리를 담당

### 💡 웹, 앱 동작방식
- 통신 프로토콜(Communication Protocol, 통신 규약)은 컴퓨터나 원거리 통신 장비 사이에서 메시지를 주고 받는 양식 및 규칙의 체계를 의미한다.
  - HTTP, HTTPS, FTP, SSL

- 최초 요청(Request)
- 최초 응답(Response)
- 추가 요청
- 추가 응답 **(이 과정에서 CSS, JS, JPG를 서버에 전달)**

### 로컬(Local) 개발 환경
- 웹 사이트를 개발할 우리의 컴퓨터 환경

## 💡 웹 표준
- 웹 표준(Web Standard)
  - 웹에서 사용되는 표준 기술이나 규칙
  - W3C의 표준화 제정 단계의 '권고안(REC)'에 해당하는 기술

##💡 W3C의 표준화 제정 단계
1. 초안(Working Draft, WD)
2. 후보권고안(Candidate Recommendation, CR)
3. 제안권고안(Proposed Recommendation, PR)
4. 권고안(W3C Recommendation,REC)

## 💡 크로스 브라우징(Cross Browsing)
- 조금은 다르게 구동되는 여러 브라우저에서, 동일한 사용자 경험(같은 화면, 같은 동작 등)을 줄 수 있도록 제작하는 기술, 방법

## 브라우저 명칭
- 창(window)
- 탭(Tab)
- 주소창(Address Bar)
- 뷰포트(Viewport) : 하나의 웹페이지가 출력(Rendering)되는 화면

##💡 웹 이미지
1. Bitmap
- 픽셀이 모여 만들어진 정보의 집합, **Raster 이미지**
- 정교하고 다양한 색상을 자연스럽게 표현, <U>**앨리어싱 현상, 품질 저하**</U>
2. Vector
- 점, 선, 면의 위치(좌표), 색상 등 수학적 정보의 형태(Shape)로 이루어진 이미지
- **앨리어싱 현상 X, 정교한 이미지(인물, 풍경사진 등) 표현 어려움**.
3. Material Design (**참고**)
- 고품질 디지털 경험을 구축할 수 있도록 Google에서 만든 디자인 시스템
4. JPG(Joint Photographic coding Experts Group)
- Full-color 와 Gray-Scale의 압축을 위해 만들어졌으며, 압축률이 훌륭해 사진이나 예술 분야에서 많이 사용.
- ### 특징
  - **손실** 압축 : 이미지가 손실되면서 압축, **반복적으로 새롭게 저장하면 색 발화**
  - 표현 색상도(**24비트**, 2^24)
  - 이미지의 품질과 **용량 쉽게 조절 가능**
  - 가장 널리 쓰이는 이미지 포맷
5. PNG(Portable Network Graphics)
- Gif의 대체 포맷으로 개발 됌.
- ### 특징
  - **비손실** 압축, 용량이 비교적 JPG보다 크다.
  - 8비트(256색상) / **24비트**(약 1600만 색상) 컬러 이미지 처리
  - Alpha Channel 지원(**투명도**)
  - W3C 권장포맷
6. GIF(Graphics Interchange Format)
- 이미지 파일 내에 이미지 및 문자열 같은 정보들을 저장.
- ### 특징
  - **비손실** 압축
  - **여러 장의 이미지를 한 개의 파일**에 담을 수 있음 ex)움짤, 애니메이션
  - **8비트 색상**(256색상)만 지원(다양한 색상 표현 x)
7. WEBP
- JPG, PNG, GIF를 모두 대체할 수 있는 구글이 개발한 이미지 포맷
- ### 특징
  - 완벽한 손실 / 비손실 압축 지원
  - GIF 같은 애니메이션 지원
  - Alpha Channel 지원
8. SVG(Scalable Vector Graphics)
- 마크업 언어(HTML/XML) 기반의 벡터 그래픽을 표현하는 포맷
- ### 특징
  - 해상도의 영향에서 자유로움
  - CSS와 JS로 제어 가능
  - 파일 및 코드 삽입 기능
