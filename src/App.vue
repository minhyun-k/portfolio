<template>
  <h2 class="Portfolio">MinHyun's PORTFOLIO</h2>
  <nav class="sticky" :class="{'backColor' : !topBtn}">
    <router-link to="/" class="menu">ABOUT</router-link>
    <span class="menuLine">|</span>
    <router-link to="/project" class="menu">PROJECT</router-link>
  </nav>
  <div class="icon_box">
    <button class="icon git" style="background-image: url('/git.svg');" @click="git()"></button>
    <button class="icon resume" style="background-image: url('/resume-50.png');" @click="downloadPdf()" ></button>
    <button class="icon top" style="background-image: url('/top-black.png');" @click="gotop()"></button>
  </div>
  <FooterComponent/>
  <router-view/>
</template>
<script>
import FooterComponent from '@/components/FooterComponent.vue'

export default{

  name:'App',
  components:{
    FooterComponent,
  },
  data(){
        return {
            topBtn: true,
            lastScrollPosition: 0
        }
    },
  mounted(){
      window.addEventListener('scroll', this.onScroll)
  },
  beforeUnmount() {
      window.removeEventListener('scroll', this.onScroll)
  },
  methods: {
    onScroll(){
      const currentScrollPosition = window.scrollY || document.documentElement.scrollTop

      if(currentScrollPosition < 0){
          return
      }
      this.topBtn = currentScrollPosition < 340
      this.lastScrollPosition = currentScrollPosition
    },
    vercel: function(){
      window.open("https:////vercel.com/minhyun-ks-projects");
    },
    git: function(){
      window.open("https://github.com/minhyun-k/minhyun-k");
    },
    downloadPdf(){
      const filePath = '/resume.pdf'


      const link = document.createElement('a');
      link.href = filePath;
      link.download = 'resume_강민현.pdf';
      link.click();
    },
    gotop(){
      window.scrollTo({top: 0, behavior:'smooth'})
    }
  }
}
</script>
<style lang="scss">
  @import "./assets/scss/res.scss";
body{margin: 0;}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #333;
  text-align: center;
  height: 3300px;
  margin: 0;
  padding: 0;
  word-break: keep-all;
  @include res('tablet'){
      height: 3400px;
    }
  @include res('mobile'){
      height: 3500px;
    }
}

nav {
}
.sticky{
  z-index: 999;
  position: sticky;
  top: 0;
  padding: 20px 0;
  transition: .2s;
  &.backColor{
    background-color: rgba(0, 0, 0, .2);
    transition: .5s;
  }
.menu{
  font-size: 20px;
  font-weight: 400;
  transition: .5s;
}
.menuLine{
  font-size: 20px;
  padding: 0 28px;
}
a {
  font-weight: bold;
  color: #333;
  text-decoration: none;

  &.router-link-exact-active {
    color: #333;
    font-weight: bold;
    padding: 4px;
    transition: .5s;
  }
}
}
ul{
  padding: 0;
}
li {
  list-style: none;
}
p{
  margin: 0;
  padding: 0;
}
.Portfolio{
  font-size: 40px;
  font-weight: bold;
  margin: 80px 0 170px;
  @include res('mobile'){
      margin: 20px 0 60px;
    }
}
// icon
.icon_box{
  z-index: 999;
  position: fixed;
  left: 3%;
  bottom: 5%;
  transform: translateX(-3%);
  gap: 20px;
  display: flex;
  flex-direction: column;
  align-items: center;
  .icon{
    width: 45px;
    height: 45px;
    border: 1px solid #ddd;
    background-color: #fff;
    border-radius: 100%;
    background-repeat: no-repeat;
    background-position: center;
    cursor: pointer;
    @include res('tablet'){
        display: none;
      }
    @include res('mobile'){
        display: none;
      }
  }
  .resume{
    background-size: 90%;
  }
  .git{
  }
  .top{
    background-size: 80%;
  }
}
</style>
