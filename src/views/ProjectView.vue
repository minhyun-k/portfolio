<template>
  <div class="project ">
    <ul class="project_list">
      <li class="project_content">
          <img class="thumb" src="/ieum_thumb.png" alt="ieum">
        <div class="txt">
          <p class="type">Team</p>
          <h2 class="title">IEUM</h2>
          <p class="skill">#Next #Scss #Zustand #Firestore #Mui</p>
            <p class="cal">2024.10.04 ~ 2024.10.30</p>
            <p class="desc">
              IEUM은 독서 활동을 기록하고, 
              원하는 도서를 검색 및 책에 대한 리뷰를 작성할 수 있는 
              도서리뷰 웹 애플리케이션입니다.
              사용자는 다양한 책을 탐색하고 자신만의 도서 목록을 관리할 수 있으며, 각 도서에 대한 상세 정보와 리뷰를 쉽게 확인할 수 있습니다.
              <br/>
              <br/>
              이 프로젝트는 사용자 친화적인 UI를 구현하려 노력했으며, 유연한 데이터 처리 구조, 데이터베이스와의 통합을 통해 효율적인 데이터를 제공을 목표로 했습니다.
              Next.js와 Firebase를 활용해 
              사용자 인증 및 데이터 저장 기능을 구현했으며, 
              React와 SCSS로 사용자가 쉽게 탐색할 수 있도록 깔끔한 UI/UX를 설계했습니다.
            </p>
          <button @click="git('github.com/minhyun-k/Book-IEUM.git')" class="git" >Github</button>
          <button @click="vercel('book-ieum.vercel.app')" class="view">View</button>
        </div>
      </li>
      <li class="project_content_r">
        <div class="project_content_box">
          <div class="txt">
          <p class="type">Team</p>
          <h2 class="title">해양생물연구센터</h2>
          <p class="skill">#HTML #Scss #JavaScript</p>
            <p class="cal">2024.06 ~ 2024.08</p>
            <p class="desc">
              한화 해양생물연구센터 사이트를 재구성한 프로젝트입니다. 기존 사이트의 관리가 제대로 이루어져 있지 않고, 노후화되어 있어 각 단점들을 보완하고 사용자에게 정보 제공을 위한 더 좋은 디자인을 목표로 했습니다.
              <br/>
              <br/>
              HTML, JavaScript, CSS만을 사용하여 구현한 해양생물연구센터 리뉴얼 사이트는 프레임워크 없이 단순한 코드로 충분한 기능을 구현하려 노력했습니다. 웹 개발의 기초적인 요소들로 사용자에게 더 나은 경험을 제공하는 것을 목표로 했습니다. 또한, 다양한 상호작용을 가능하게 하여 심플하면서도 직관적인 사용자 인터페이스를 제공합니다.
            </p>
            <button @click="git('github.com/minhyun-k/B-project.git')" class="git" >Github</button>
            <button @click="vercel('b-project-lilac.vercel.app/')" class="view">View</button>
        </div>
            <img class="thumb" src="/aqua_thumb.jpg" alt="aqua">
        </div>
      </li>
      <li class="project_content">
        <div class="thumb_box">
          <img class="thumb" src="/movie_thumb.jpg" alt="movie">
        </div>
        <div class="txt">
          <p class="type">Personal</p>
          <h2 class="title">YFLIX</h2>
          <p class="skill">#React.js #Scss #Axios(TMDB API) </p>
            <p class="cal">2024.07.24~2024.09.05</p>
            <p class="desc">
              YFLIX는 영화 팬들을 위한 영화 탐색 애플리케이션을 클론 코딩한 프로젝트로, 사용자가 다양한 영화의 상세 정보를 탐색할 수 있는 플랫폼입니다. 
              영화 포스터, 줄거리, 평점 등의 정보를 한눈에 볼 수 있으며, 인기 영화와 최신 개봉작을 확인할 수 있는 기능을 제공합니다.
              <br/>
              <br/>
              React 프레임워크를 사용하였으며, 이 프로젝트는 외부 영화 API와의 통합을 통해 실시간으로 업데이트되는 영화 정보를 제공하며, 다양한 필터와 정렬 옵션으로 사용자가 관심 있는 영화 정보를 쉽게 찾을 수 있도록 합니다. 데이터 시각화와 인터페이스 설계를 통해 사용자 참여를 유도하고, API 데이터를 효율적으로 관리하는 역량을 보여주는 프로젝트입니다.
            </p>
            <button @click="git('github.com/minhyun-k/movie.git')" class="git" >Github</button>
            <button @click="vercel('vercel.com/minhyun-ks-projects/movie')" class="view">View</button>
        </div>
      </li>
      <li class="project_content_r">
        <div class="project_content_box">
          <div class="txt">
          <p class="type">Personal</p>
          <h2 class="title">Portfolio</h2>
          <p class="skill">#Vue.js #Scss</p>
            <p class="cal">2024.11.18~</p>
            <p class="desc">
              이 포트폴리오는 제가 Vue.js를 이용하여 개발한 다양한 웹 애플리케이션을 소개하는 공간입니다. 반응형 디자인을 통해 모든 디바이스에서 원활하게 작동하게 만들었습니다.
              <br/>
              <br/>
              각 프로젝트는 사용자가 필요로 하는 정보를 직관적으로 제공하고, 성능과 확장성을 고려한 코드로 구성되었습니다. 제 포트폴리오는 프론 트엔드 개발자로서의 경험과 역량을 보여주는 작품들입니다.
            </p>
            <button @click="git('github.com/minhyun-k/portfolio.git')" class="git" >Github</button>
            <button @click="vercel('portfolio-peach-eight-19.vercel.app')" class="view">View</button>
        </div>
          <div class="thumb_box">
            <img class="thumb" src="/portfolio.png" alt="portfolio">
          </div>
        </div>
      </li>
      <li class="project_content">
        <div class="thumb_box">
          <img class="thumb" src="/todo_thumb.jpg" alt="todos">
        </div>
        <div class="txt">
          <p class="type">Personal</p>
          <h2 class="title">todos</h2>
          <p class="skill">#React #Scss #express #mongoDB</p>
            <p class="cal">2024.09.16~2024.09.30</p>
            <p class="desc">
              Todos는 직관적인 사용자 인터페이스와 간단한 사용법을 제공하는 작업 관리 애플리케이션으로, 사용자들이 일정을 관리하고 생산성을 높일 수 있도록 돕습니다. 사용자는 새 작업을 추가, 수정, 삭제할 수 있으며, 작업 완료 여부를 확인하여 진행 상황을 간편하게 관리할 수 있습니다.
              <br/>
              <br/>
              React와 Express를 활용하여 프로젝트를 진행했습니다.
              이 프로젝트는 CRUD 기능을 구현하고 로컬 저장소와 같은 기술을 활용해 데이터를 지속적으로 관리하며, 
              상태 관리와 데이터 조작을 통해 사용자 중심의 기능을 최적화하려고 노력했습니다.
            </p>
            <button @click="git('github.com/minhyun-k/todos.git')" class="git" >Github</button>
            <button @click="vercel('todos-drab-delta.vercel.app')" class="view">View</button>
        </div>
      </li>
      <li class="project_content_r">
        <div class="project_content_box">
          <div class="txt">
          <p class="type">Personal</p>
          <h2 class="title">API-NEWS</h2>
          <p class="skill">#Vue.js #Scss #express #Axios(딥서치api)</p>
            <p class="cal">2024.10.21~2024.10.25</p>
            <p class="desc">
              API News는 실시간 뉴스 API를 활용해 최신 뉴스 콘텐츠를 제공하는 웹 애플리케이션입니다. 사용자는 원하는 주제의 뉴스를 손쉽게 탐색할 수 있으며, 다양한 카테고리와 키워드를 통해 관심 있는 기사를 쉽게 찾을 수 있습니다.
              <br/>
              <br/>
              Vue.js와 Express를 활용해 기능을 구현했으며,
              API와의 통합으로, 빠르게 업데이트되는 뉴스 콘텐츠를 사용자에게 제공하여 시의성을 유지하며,
              이 프로젝트는 API 통합, 데이터 페칭, 그리고 효율적인 상태 관리를 통해 실시간 데이터를 다루는 것을 중점으로 진행했습니다.
            </p>
            <button @click="git('github.com/minhyun-k/News.git')" class="git" >Github</button>
            <button @click="vercel('apinews-virid.vercel.app')" class="view">View</button>
        </div>
          <div class="thumb_box">
            <img class="thumb" src="/news__thumb.jpg" alt="news">
          </div>
        </div>
      </li>
    </ul>
  </div>
</template>

<script lang="ts">
export default{
methods: {
  vercel: function(url:string){
    window.open(`https://${url}`);
    },
  git: function(url:string){
    window.open(`https://${url}`);
  },
}
}
</script>

<style lang="scss">
  @import "../assets/scss/res.scss";




  .project{
    text-align: inherit;
    .project_list{
      padding: 0;
      .project_content{
        max-width: 1200px;
        margin: 40px auto;
        display: flex;
        justify-content: center;
        @include res('tablet'){
          display: block;
        }
        @include res('mobile'){
          display: block;
        }

        .thumb{
          width: 590px;
          height: 510px;
          object-fit: cover;
          @include res('mobile'){
            width: 300px;
            height: 400px;
          }
        }
        .txt{
          max-height: 510px;
          width: 500px;
          text-align: left;
          margin-left: 60px;
          position: relative;
          @include res('tablet'){
            width: 590px;
            margin: 0 auto;
            padding-bottom: 60px;
          }
          @include res('mobile'){
            width: 300px;
            margin: 0 auto;
            padding-bottom: 60px;
          }
          .type{
            font-size: 16px;
            margin: 20px 0 32px;
            font-weight: bold;
            @include res('tablet'){
              margin-bottom: 20px;
            }
            @include res('mobile'){
              margin-bottom: 20px;
            }
          }
          .title{
            font-size: 48px;
            font-weight: bolder;
            margin: 0;
            padding-bottom: 8px;
            @include res('mobile'){
              font-size: 36px;
            }
          }
          .skill{
            font-size: 16px;
            word-spacing: 20px;
            margin-bottom: 52px;
            @include res('tablet'){
              margin-bottom: 32px;
            }
            @include res('mobile'){
              margin-bottom: 32px;
            }
          }
          .cal{
            font-size: 16px;
            font-weight: bold;
          }
          .desc{
            font-size: 16px;
            color: #555555;
            @include res('mobile'){
              font-size: 14px;
            }
          }
          .git{
            top: 100%;
            left: 0%;
            transform: translate(0%,-100%);
          }
          .view{
            padding: 10px 57.71px;
            color: white;
            background-color: black;
            top: 100%;
            left: 25%;
            transform: translate(25%,-100%);
            @include res('mobile'){
              top: 100%;
              left: 32%;
              transform: translate(32%, -100%);
              padding: 10px 37.71px;
            }
          }

          button{
            font-size: 16px;
            font-weight: bold;
            padding: 10px 50px;
            border: 1px solid #111;
            border-radius: 10px;
            background-color: #fff;
            position: absolute;
            cursor: pointer;
            @include res('mobile'){
              padding: 10px 30px;
            }
          }
        }
      }
    }
  }

  .project{
    text-align: inherit;
    .project_list{
      .project_content_r{
        padding: 40px 0;
        .project_content_box{
          max-width: 1200px;
          margin: 40px auto;
          display: flex;
          justify-content: center;
          position: relative;
          @include res('tablet'){
            align-items: center;
            flex-direction: column-reverse;
          }
          @include res('mobile'){
            align-items: center;
            flex-direction: column-reverse;
          }
          .thumb{
            width: 590px;
            height: 510px;
            object-fit: cover;
            @include res('mobile'){
              width: 300px;
              height: 400px;
            }
          }
          .txt{
          max-height: 510px;
          width: 500px;
          text-align: left;
          margin-right: 60px;
          position: relative;
          @include res('tablet'){
              width: 590px;
              padding-bottom: 60px;
              margin: 0 auto;
            }
          @include res('mobile'){
              width: 300px;
              padding-bottom: 60px;
              margin: 0 auto;
            }
          .type{
            font-size: 16px;
            margin: 20px 0 32px;
            font-weight: bold;
            @include res('tablet'){
              margin-bottom: 20px;
            }
            @include res('mobile'){
              margin-bottom: 20px;
            }
          }
          .title{
            font-size: 48px;
            font-weight: bolder;
            margin: 0;
            padding-bottom: 8px;
            @include res('mobile'){
              font-size: 36px;
            }
          }
          .skill{
            font-size: 16px;
            word-spacing: 20px;
            margin-bottom: 52px;
            @include res('tablet'){
              margin-bottom: 32px;
            }
            @include res('mobile'){
              margin-bottom: 32px;
            }
          }
          .cal{
            font-size: 16px;
            font-weight: bold;
          }
          .desc{
            font-size: 16px;
            color: #555555;
            @include res('mobile'){
              font-size: 14px;
            }
          }
          .git{
            top: 100%;
            left: 0%;
            transform: translate(0%,-100%);
          }
          .view{
            padding: 10px 57.71px;
            color: white;
            background-color: black;
            top: 100%;
            left: 25%;
            transform: translate(25%,-100%);
            @include res('mobile'){
              padding: 10px 37.71px;
              top: 100%;
              left: 32%;
              transform: translate(32%, -100%);
            }
          }

          button{
            font-size: 16px;
            font-weight: bold;
            padding: 10px 50px;
            border: 1px solid #111;
            border-radius: 10px;
            background-color: #fff;
            position: absolute;
            cursor: pointer;
            @include res('mobile'){
              padding: 10px 30px;
            }
          }
        }
        }
      }
    }
  }



  
</style>