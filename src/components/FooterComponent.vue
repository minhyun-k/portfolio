<template >
    <div class="footer" :class="{'hidden' : !showFooter}">
        <ul class="menu">
            <li class="menu_list">
                <button class=" f_icon f_git" style="background-image: url('/git.svg');" @click="git()">
                </button>
            </li>
            <li class="menu_list">
                <button class="f_icon f_vercel" style="background-image: url('/vercel.png');" @click="vercel()">
                </button>
            </li>
            <li class="menu_list">
                <button class="f_icon f_resume" style="background-image: url('/resume-50.png');" @click="downloadPdf()" >
                </button>
            </li>
            <li class="menu_list">
                <button class="f_icon f_top" style="background-image: url('/top-black.png');" @click="gotop()">
                </button>
            </li>
        </ul>
    </div>
</template>
<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
    data(){
        return {
            showFooter: true,
            lastScrollPosition: 0
        }
    },
    mounted(){
        window.addEventListener('scroll', this.onScroll)
    },
    beforeUnmount() {
        window.removeEventListener('scroll', this.onScroll)
    },  
    methods:{
        onScroll(){
            const currentScrollPosition = window.scrollY || document.documentElement.scrollTop

            if(currentScrollPosition < 0){
                return
            }
            this.showFooter = currentScrollPosition < this.lastScrollPosition
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
})
</script>
<style lang="scss">
    @import "../assets/scss/res.scss";

    .footer{
        display: none;
    }

    @include res('tablet'){
    .footer{
        z-index: 999;
        display: block;
        background-color: #fff;
        margin: 0 auto;
        padding: 20px 0;
        position: fixed;
        width: 100%;
        top: 100%;
        left: 50%;
        transform: translate(-50%, -100%);
        border-top: 1px solid #555;
        &.hidden{
            top: 150%;
        }
        .menu{
            margin: 0;
            display: flex;
            align-items: center;
            justify-content: space-between;
            .menu_list{
                width: 25%;
                height: 40px;
                .f_icon{
                    background-color: #fff;
                    border: none;
                    width: 40px;
                    height: 40px;
                    background-repeat: no-repeat;
                    background-position: center;
                    background-size: contain;
                }
                .f_git{}
                .f_vercel{}
                .f_resume{}
                .f_top{}
            }
        }
    }
}
    @include res('mobile'){
    .footer{
        z-index: 999;
        display: block;
        background-color: #fff;
        margin: 0 auto;
        padding: 20px 0;
        position: fixed;
        width: 100%;
        top: 100%;
        left: 50%;
        transform: translate(-50%, -100%);
        border-top: 1px solid #555;
        transition: 0.5s;
        &.hidden{
            top: 120%;
            transition: 0.7s;
        }
        .menu{
            margin: 0;
            display: flex;
            align-items: center;
            justify-content: space-between;
            .menu_list{
                width: 25%;
                height: 40px;
                .f_icon{
                    background-color: #fff;
                    border: none;
                    width: 40px;
                    height: 40px;
                    background-repeat: no-repeat;
                    background-position: center;
                    background-size: contain;
                }
                .f_git{}
                .f_vercel{}
                .f_resume{}
                .f_top{}
            }
        }
    }
}
</style>