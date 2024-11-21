<template>
  <nav class="header">
    <h2 class="Portfolio">Portfolio</h2>
    <router-link to="/" class="menu">ABOUT</router-link> 
    <span class="menuLine">|</span>
    <router-link to="/project" class="menu">PROJECT</router-link>
    <button class="icon git" style="background-image: url('/git.svg');" @click="git()"></button>
    <button class="icon vercel" style="background-image: url('/vercel.png');" @click="vercel()"></button>
    <button class="icon resume" style="background-image: url('/resume-50.png');" @click="downloadPdf()" ></button>
    <button class="icon top" style="background-image: url('/top-black.png');" @click="gotop()"></button>
    <FooterComponent/>
  </nav>
  <router-view/>
</template>
<script>
import FooterComponent from '@/components/FooterComponent.vue'

export default{

  name:'App',
  components:{
    FooterComponent,
  },
  methods: {
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

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #333;
  text-align: center;
  margin: 0;
  padding: 0;
}

nav {
  padding: 60px;
  padding-bottom: 80px;

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
  margin: 20px 0 120px;
  @include res('mobile'){
      margin: 20px 0 60px;
    }
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
// icon
.icon{
  z-index: 999;
  width: 45px;
  height: 45px;
  border: 1px solid #ddd;
  border-radius: 100%;
  background-repeat: no-repeat;
  position: fixed;
  left: 3%;
  transform: translateX(-3%);
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
  top: 72%;
  transform: translateY(-72%);
  background-size: 90%;
}
.git{
  top: 78%;
  transform: translateY(-78%);
}
.vercel{
  top: 84%;
  transform: translateY(-84%);
  background-size: 60%;
}
.top{
  top: 90%;
  transform: translateY(-90%);
  background-size: 80%;
}
</style>
