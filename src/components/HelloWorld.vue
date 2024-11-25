<template>
  <div>
    <div class="banner">
      <div class="intro">
        <h2 class="intro_title">안녕하세요<br/>저는 프론트 엔드 개발자 강민현입니다.</h2>
        <p class="intro_txt">
          끝이 없는 배움은 새로운 것을 맞이하는 즐거움이라고 생각합니다.<br/>
          즐겁게 지나온 저의 발자국을 소개하겠습니다.<br/>
          저의 웹 포트폴리오를 찾아주셔서 감사합니다.
        </p>
      </div>
      <div class="profile">
        <div class="profile_img" style="background-image: url('/kmh.jpg');"></div>
        <p class="birth">1996.05.14</p>
        <p class="phone">010-3840-5074</p>
        <p class="e-mail">alsgus3074@gmail.com</p>
      </div>
    </div>
    
    <h2 class="title">INTERVIEW<span class="title_line"></span></h2>

    <div class="interview">
      <div class="interview_box">
        <h3 class="interview_title">웹 개발자를 선택한 이유는?</h3>
        <p class="interview_txt1 itxt">
          실생활에서 온라인 환경을 직접 경험하면서 온라인 환경 구축과 작동에 대한 호기심을 항상 가지고 있었습니다.
          평소 궁금하던 부분을 풀고 새로운 환경을 직접 만들 수 있는 부분에서 흥미를 느꼈습니다.
        </p>
        <p class="interview_txt2 itxt">
          온라인 환경은 이제 우리의 삶에 당연한 부분으로 다가왔고, 앞으로도 온라인 환경의 중요성은 더욱 강조될 것이라고 생각하여 웹 개발자가 되려고 했습니다.
        </p>
      </div>
      <div class="interview_box">
        <h3 class="interview_title">일에 있어 중요하게 생각하는 것은?</h3>
        <p class="interview_txt1 itxt">
          새로운 것을 배우고 맞이하는 것을 중요시 하며, 배움을 통한 성장이 다른 성장의 발판이 되도록 역량으로 쌓는 것이 중요하다고 생각합니다.
        </p>
        <p class="interview_txt2 itxt">
          또한 다양한 협업이 중시되는 요즘 공통된 목표를 위한 협업과정에서 이해관계자들과의 배려와 이해, 맡은 업무에 대한 책임감과 그 책임감에 대한 인지가 중요하다고 생각합니다. 
        </p>
      </div>
      <div class="interview_box">
        <h3 class="interview_title">나의 장점은?</h3>
        <p class="interview_txt1 itxt">
          새로운 것을 받아들이고 배우는 데 거부감이 없으며, 받아들이는 과정에 흥미를 느끼고 빠르게 익힙니다.
        </p>
        <p class="interview_txt2 itxt">
          또한 상대방에 대한 배려를 중요시하며, 누군가를 이해하는 것을 좋아합니다. 이런 성격으로 공통의 목표를 위해 한 팀이 유지되고 함께 그것을 이룰 때 큰 성취감을 느낍니다.
        </p>
      </div>
    </div>

    <div class="skills">
      <h2 class="title">SKILLS<span class="title_line2"></span></h2>
      <div class="skill_box" :class="{ active: isActive==1 }">
        <ul class="skill_title" @click="s_act(1)">
          <li class="s_t">#HTML5</li>
          <li class="s_t">#CSS3</li>
          <li class="s_t">#SASS</li>
          <li class="s_t">#FIGMA</li>
        </ul>
        <ul class="skill_txt">
          <li class="s_txt">
            웹 페이지의 기본 구조를 정의하며, 효율적인 마크업을 통해 접근성을 고려한 HTML 설계를 할 수 있습니다.</li>
          <li class="s_txt">
            SASS를 이용해 복잡한 스타일을 모듈화하고 유지와 관리가 쉬운 코드로 작성하려고 노력합니다.</li>
          <li class="s_txt">반응형 웹 디자인을 할 수 있습니다.</li>
          <li class="s_txt">웹 표준을 지키고 웹 접근성을 높이려고 노력합니다.</li>
        </ul>
      </div>
      <div class="skill_box" :class="{ active: isActive==2 }">
        <ul class="skill_title" @click="s_act(2)">
          <li class="s_t">#JavaScript</li>
          <li class="s_t">#TypeScript</li>
        </ul>
        <ul class="skill_txt">
          <li class="s_txt">
            웹 애플리케이션에 동적인 기능을 추가하며, 다양한 JavaScript 문법을 통해 효율적이고 확장성 있는 코드를 작성할 수 있습니다.</li>
          <li class="s_txt">
            실행 컨텍스트, 호출 스택과 이벤트 루프의 동작 원리를 이해하여 사용하고, 코드의 가독성을 높이고 유지보수성을 향상시키려 노력합니다.</li>
          <li class="s_txt">
            TypeScript를 이용하여 JavaScript에 정적 타입을 부여해 코드의 안정성과 가독성을 높이며, 대규모 애플리케이션 개발 시 유지보수가 용이하도록 합니다.</li>
        </ul>
      </div>
      <div class="skill_box" :class="{ active: isActive==3 }">
        <ul class="skill_title" @click="s_act(3)">
          <li class="s_t">#REACT</li>
          <li class="s_t">#NEXT.js</li>
          <li class="s_t">#VUE.js</li>
        </ul>
        <ul class="skill_txt">
          <li class="s_txt">
            합리적인 방식으로 컴포넌트를 분리하여 컴포넌트의 재사용성을 높입니다. Hooks를 활용한 상태 관리, Zustand, Redux, Context API를 통한 전역 상태 관리, 효율적인 가상 DOM 활용으로 성능을 최적화합니다. 
          </li>
          <li class="s_txt">
            CSR, ISG, SSG, SSR 4가지 렌더링 기법에 대해 이해하고, 각 페이지에 적절한 렌더링 기법을 선택하여 사용할 수 있으며, 동적 라우팅을 통한 효율적인 페이지 관리와 API 라우트 기능을 이용할 수 있습니다.
          </li>
          <li class="s_txt">
            Vue의 템플릿 문법과 v-if, v-for 같은 디렉티브를 활용해 데이터 바인딩을 쉽게 관리하고, 컴포넌트 기반 설계를 통해 일관성과 유지보수를 용이하게하고, Vuex를 활용해 글로벌 상태를 관리하여 데이터의 흐름을 관리합니다.
          </li>
        </ul>
      </div>
      <div class="skill_box" :class="{ active: isActive==4 }">
        <ul class="skill_title" @click="s_act(4)">
          <li class="s_t">#Firebase</li>
          <li class="s_t">#Express</li>
        </ul>
        <ul class="skill_txt">
          <li class="s_txt">
            express.json() 같은 기본 미들웨어와 함께 morgan 등 추가 미들웨어를 활용해 요청, 인증, 오류 처리 등을 관리할 수 있으며, 다양한 URL패턴을 처리하는 유연한 라우팅 시스템을 통해 클라이언트 요청을 쉽게 처리하고, 모듈화를 통해 코드 유지보수를 향상시키려 노력합니다. 
          </li>
          <li class="s_txt">
            Firestore 및 Realtime Database, NoSQL  방식의 데이터베이스로 실시간 데이터 업데이트를 지원하며, 복잡한 데이터를 손쉽게 관리하고 실시간 데이터 업데이트가 필요한 애플리케이션을 구축합니다.
          </li>
        </ul>
      </div>
      <div class="skill_box" :class="{ active: isActive==5 }">
        <ul class="skill_title" @click="s_act(5)">
          <li class="s_t">#Github</li>
          <li class="s_t">#Vercel</li>
        </ul>
        <ul class="skill_txt">
          <li class="s_txt">
            협업과 버전 관리를 위한 중요한 도구로서, 브렌치 전략을 통한 코드 관리, Pull Request를 통한 코드 리뷰 등 Git 명령어와 워크플로우를 통해 프로젝트를 체계적으로 관리할 수 있습니다.
          </li>
          <li class="s_txt">
          Next.js와의 최적화된 통합을 통해 쉽고 빠르게 애플리케이션을 배포합니다. 자동 빌드 및 베포를 통한 CI/CD를 구축합니다.
          </li>
        </ul>
      </div>
    </div>

    <h2 class="title">EDUCATION<span class="title_line3"></span></h2>

    <div class="education">
      <div class="edu">
        <p class="cal">2017.03 ~ 2023.08</p>
        <p class="where">단국대학교</p>
        <p class="what">상담학과&경영학과</p>
      </div>
      <div class="edu">
        <p class="cal">2024.05~2024.11</p>
        <p class="where">그린컴퓨터아카데미</p>
        <p class="what">
          프로젝트기반 프론트엔드 (React,Vue) 웹&앱 
          SW개발자 양성과정
        </p>
      </div>
      <div class="edu">
        <p class="cal">2024.12~</p>
        <p class="where">OOO 입사</p>
        <p class="what"></p>
      </div>
    </div>
  </div>
</template>

<style scoped lang="scss">
  @import "../assets/scss/res.scss";

  .banner{
    background-color: rgba(0, 0, 0, .02);
    text-align: center;
    padding: 80px;
    margin: 0;
    @include res('mobile'){
      padding: 40px;
    }
    .intro{
      .intro_title{
        font-size: 28px;
        line-height: 40px;      
        text-decoration-line: underline;
        font-weight: 500;
        text-underline-offset: 5px;
        margin: 0;
        @include res('mobile'){
          font-size: 20px;
          line-height: 30px;
          padding-bottom: 20px;
        }
      }
      .intro_txt{
        padding-top: 20px;
        line-height: 28px;
        margin: 0 auto;
        font-size: 18px;
        max-width: 600px;
        @include res('mobile'){
          font-size: 16px;
          line-height: 24px;
          word-break: keep-all;
        }
      }
    }
    .profile{
      
      .profile_img{
        margin: 40px auto 20px;
        max-width: 156px;
        height: 156px;
        border-radius: 100%;
        background-size: contain;
        background-repeat: no-repeat;
        background-position: center 10px;
        background-color: #fff;
        border: 1px solid #eee;
      }
      .birth{
        font-size: 18px;
        margin-bottom: 8px;
      }
      .phone{
        font-size: 18px;
        margin-bottom: 8px
      }
      .e-mail{
        font-size: 18px;
      }
    }
  }
  .title{
    margin: 120px 0 80px;
    font-size: 36px;
    font-weight: 500;
    // text-decoration: line-through solid #333333 1px ;
    position: relative;
    @include res('mobile'){
          margin: 60px 0 20px;
        }
  }
  .title_line{
    display: inline-block;
    width: 242px;
    height: 1px;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    background-color: #111;
    position: absolute;;
  }
  .title_line2{
    display: inline-block;
    width: 162px;
    height: 1px;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    background-color: #111;
    position: absolute;;
  }
  .title_line3{
    display: inline-block;
    width: 248px;
    height: 1px;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    background-color: #111;
    position: absolute;;
  }
  .interview{
    display: flex;
    align-content: center;
    justify-content: center;
    gap: 24px;
    margin-bottom: 80px;
    @include res('tablet'){
          flex-wrap: wrap;
    }
    @include res('mobile'){
          flex-wrap: wrap;
          margin: 0 20px;
    }
    .interview_box{
      border: 1px solid rgba(0, 0, 0, .2);
      border-radius: 16px;
      max-width: 390px;
      .interview_title{
        padding: 15px 0;  
        font-size: 18px;
        font-weight: 500;
        color: #fff;
        background-color: #111;
        text-decoration-line: center;
        margin: 24px;
        @include res('tablet'){
          font-size: 16px;
        }
        @include res('mobile'){
          font-size: 16px;
        }
      }
      .itxt{
        font-size: 16px;
        line-height: 28px;
        padding: 0 24px;
        @include res('tablet'){
          font-size: 14px;
          text-align: left;
        }
        @include res('mobile'){
          font-size: 14px;
          text-align: left;
        }
      }
      .interview_txt1{
        margin-bottom: 20px;

      }
      .interview_txt2{
        margin-bottom: 24px;
      }
    }
  }
  .skills{
    background-color: rgba(0, 0, 0, .02);    
    padding: 10px 80px 80px;
    text-align: center;
    @include res('mobile'){
      padding: 10px 20px 40px;
    }
    .skill_box{
      max-width: 1200px;
      text-align: left;
      margin: 0 auto;
      .skill_title{
        margin: 0;
        border-top: 1px solid black;
        display: flex;
        align-items: center;
        gap: 20px;
        padding: 24px;
        position: relative;
        cursor: pointer;
        &::after{
          content: url(/public/down.svg);
          position: absolute;
          left: 98%;
          transform: translateX(-100%);
        }
        .s_t{
          font-size: 18px;
          font-weight: bold;
          @include res('mobile'){
            font-size: 14px;
          }
        }
      }
      &.active .skill_title::after{
          content: url(/public/up.svg);
          position: absolute;
          left: 98%;
          transform: translateX(-100%);
        }
      &.active .skill_txt{
        display: block;
        transition: .3s;
      }
      .skill_txt{
        background-color: rgba(0, 0, 0, .03);
        padding: 44px;
        margin: 0;
        display: none;
        transition: .3s;
        .s_txt{
          list-style-type: square;
          font-size: 16px;
          line-height: 32px;
          @include res('mobile'){
            font-size: 14px;
            line-height: 24px;
          }
        }
      }
    }
  }
  .education{
    border-top: 3px solid #111;
    padding: 40px 0 120px;
    max-width: 1200px;
    display: flex;
    align-items: center;
    justify-content: space-around;
    position: relative;
    margin: 0 auto 40px;
    @include res('mobile'){
      margin: 40px 20px 80px;
      border: 1px solid #ddd;
      padding: 10px 20px 20px;
      display: block;
    }
    .edu{
      width: 33.33%;
      @include res('mobile'){
        width: 100%;
        padding-bottom: 0;
      }
    }
    .cal{
      font-size: 24px;
      font-weight: bold;
      @include res('tablet'){
          font-size: 16px;
        }
      @include res('mobile'){
          font-size: 16px;
          margin-top: 10px;
        }
    }
    .where{
      font-size: 16px;
      font-size: 500;
      @include res('tablet'){
          font-size: 14px;
        }
      @include res('mobile'){
          font-size: 14px;
        }
    }
    .what{
      font-size: 16px;
      @include res('tablet'){
          font-size: 14px;
        }
      @include res('mobile'){
          font-size: 14px;
        }
    }
  }
</style>

<script lang="ts">
import { defineComponent } from 'vue'
// import data from "../assets/data.json"

export default defineComponent({
  data(){
    return {isActive:1}
  },
  methods: {
    s_act(num: number) : void{
      this.isActive = num;
    }
  }

})
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
