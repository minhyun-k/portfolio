<div align="center">

<!-- logo -->
<img src="https://github.com/minhyun-k/Book-IEUM/blob/main/public/loading-1.png" width="400" height="400"/>

### Portfolio 🖍️

</div> 

## 📝 프로젝트 소개


**Portfolio**는 개인 개발자의 포트폴리오 웹사이트로, 본인의 기술 스택, 프로젝트, 경력 등을 효과적으로 소개하는 공간입니다. 이 웹사이트는 **Vue.js**를 활용하여 제작되었으며, **Vercel**에 배포되어 있습니다. 디자인은 간결하고 직관적인 방식으로 사용자의 경험을 중시하며, 모바일에서도 최적화되어 누구나 쉽게 확인할 수 있습니다.

- **목적**: 자신을 소개하는 디지털 포트폴리오를 제공하여, 개발자로서의 경력과 역량을 온라인에서 한눈에 보여줄 수 있도록 합니다.
- **특징**: 다양한 프로젝트 링크와 설명을 제공하며, 자신의 스킬셋과 기술 스택을 명확히 나타낼 수 있는 기능을 제공합니다.
- **학습 목표**: 포트폴리오 제작을 통해 **Vue.js**, **Vercel**을 활용한 웹사이트 개발 경험을 쌓습니다.

---

[**배포 사이트 바로가기**](https://portfolio-peach-eight-19.vercel.app/)  
[**GitHub Repository 바로가기**](https://github.com/minhyun-k/portfolio.git)
<br />

## 🗓 프로젝트 일정
**총 일정 2024.06 ~ 2024.08**



<br />
## 🛠 화면 구성

|화면 명|
|:---:|
|로딩 화면|
|<img src="https://github.com/minhyun-k/Book-IEUM/blob/main/public/loading.gif" width="450"/>|
|처음 어플리케이션 실행 시 로딩화면 출력|
|메인 홈|
|:---:|
|<img src="https://github.com/minhyun-k/Book-IEUM/blob/main/public/Home.gif" width="450"/>|
|홈 화면은 서버요청을 통해 베스트셀러, 신간 등 카테고리에 맞는 데이터가 출력되어 사용자가 도서 목록을 확인할 수 있습니다.|
|도서목록|
|:---:|
|<img src="https://github.com/minhyun-k/Book-IEUM/blob/main/public/list.gif" width="450"/>|
|홈 화면에서 각 카테고리별 더보기 클릭시, 혹은 헤더 메뉴 클릭시 각 카테고리에 맞는 도서 목록이 페이지에 출력됩니다.|
|상세페이지|
|:---:|
|<img src="https://github.com/minhyun-k/Book-IEUM/blob/main/public/detail.gif" width="450"/>|
|홈, 도서목록에서 사용자가 관심있는 도서 컨텐츠를 클릭 시, 클릭한 도서의 상세정보가 포함된 페이지가 열립니다. 이 페이지에서는 도서의 상세내용, 북마크, 코멘트 작성이 가능하며, 베스트셀러의 경우 베스트 순위, 신간의 경우 신간도서 표시가 제공됩니다.|
|북마크 등록 및 코멘트 작성|
|:---:|
|<img src="https://github.com/minhyun-k/Book-IEUM/blob/main/public/detail2.gif" width="450"/>|
|북마크 클릭시 '읽는중', '읽고싶어요' 등록 가능, firebase를 통해 각 로그인한 사용자 개인 북마크 기능 활성화, 코멘트 작성 시 별점과 리뷰(댓글형식)가 표시됩니다.|
|마이페이지|
|:---:|
|<img src="https://github.com/minhyun-k/Book-IEUM/blob/main/public/mypage.gif" width="450"/>|
|로그인 시 firebase를 사용하여, 각 사용자가 사용한 북마크와 코멘트가 출력되어 사용자의 경험, 히스토리를 확인할 수 있습니다.|

<br />

## ⚙ 기술 스택

이 프로젝트는 다양한 최신 기술을 활용하여 구현되었습니다.


- **Frontend**: Vue.js, JavaScript, HTML5, CSS3  
- **배포**: Vercel  
- **GitHub**: 버전 관리 및 협업 도구

<br />

## :wrench: 주요 기능 및 특징

### 1) **자기소개 페이지**
- **설명**: 웹사이트 방문자에게 개발자로서의 자기소개와 경력을 간략히 제공합니다.
- **기능**: 이름, 직무, 간단한 이력 및 기술 스택을 한눈에 보여주는 카드 형태로 구성되어 있습니다.

### 2) **프로젝트 갤러리**
- **설명**: 사용자가 진행한 다양한 프로젝트들을 소개하는 섹션입니다.
- **기능**: 각 프로젝트는 제목, 기술 스택, 배포 링크, GitHub 링크 등을 포함하며, 프로젝트 상세 정보를 제공하는 페이지로 연결됩니다.

### 3) **기술 스택 섹션**
- **설명**: 개발자가 주로 사용하는 기술을 시각적으로 보여주는 부분입니다.
- **기능**: 아이콘과 함께 각 기술의 설명을 제공하며, 각 기술의 사용 경험을 바탕으로 구체적인 설명을 덧붙여 개발자의 능력을 강조합니다.

### 4) **반응형 디자인**
- **설명**: 다양한 화면 크기에서 최적화된 디자인을 제공합니다.
- **기술 사용**: **CSS Grid**와 **Flexbox**를 활용하여 레이아웃을 구현하고, **Media Queries**로 반응형 웹사이트를 구축합니다.

---

<br />

