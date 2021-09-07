<template>
  <div id="app">
    <img v-if="btnFlag" class="go-top" src="./assets/img/backTop.png" @click="backTop">
    <TopNav  @parentOpen="childOpen"  @notLogin="back"  @parentLogin="childLogin" v-show="navShow"></TopNav>  
    <br><br>
    <TopNav v-if="check" style="position: fixed; top: 0%; width:100% ;z-index: 1000; " @parentLogin="childLogin"  @notLogin="back"></TopNav>
    <div v-show="check" class="kailong" @click="reveal"></div>
    <side-nav @parentClose="childClose"  v-if="isShowed"  :class="isShowed==true?'goLeft':'goBack'" style="z-index:10000"></side-nav>
  </div>
  <router-view />
  
  <div class="foot1" v-show="login">
    <div class="mulu1">
      <br>
      <br>
      <p>aboutBATTLEFIELD</p><br><br>
      <ul class="footnav">
        <li>
          <ul>
            <router-link to="/games" @click="back">历代游戏</router-link>
          </ul>
        </li>
        <li>
          <a href="https://baike.baidu.com/item/DICE/7456761?fr=aladdin" target="new" @click="back">开发商</a>
        </li>
        <li>
          <a href="https://baike.baidu.com/item/%E5%AF%92%E9%9C%9C%E5%BC%95%E6%93%8E/8391328?fr=aladdin" target="new" @click="back">寒霜引擎</a>
        </li>
        <li>
          <a href="https://answers.ea.com/t5/Battlefield/ct-p/battlefield"  @click="back" target="new">官方论坛</a>
        </li>
      </ul>
    </div>
    <div class="mulu2" >
      <img src="./assets/img/foot.png">
    </div>
  </div>
  <div class="foot2" v-show="login" >
    <br>

    <br>
    <br>
    有建议？请联系我们：2276001806@qq.com
  </div>
</template>

<style>
  @import './assets/css/reset.css';
</style>

<script>
  // @ is an alias to /src
  //使用其他组件
  import TopNav from '@/components/TopNav.vue'
  import LunBo from '@/components/LunBo.vue'
  import LunBou from '@/components/LunBou.vue'
  import SideNav from '@/components/SideNav.vue'
  
  export default {
    name: 'app',
    data: function () {
      return {
        check: false,
        btnFlag:false,
        isShowed:false,
        flag:true,
        login:true,
        navShow:true
      }
    },
    components: {
      TopNav,
      LunBo,
      LunBou,
      SideNav
    },
    mounted() {
      window.addEventListener('scroll', this.scroll);
      window.addEventListener('scroll', this.scrollToTop);
    },
    destroyed() {
      window.removeEventListener('scroll', this.scrollToTop)
    },
    methods: {
      scroll() {
        let scrollTop =
          window.pageYOffset ||
          document.documentElement.scrollTop ||
          document.body.scrollTop;
        if(scrollTop==0){this.flag=true}
        if (scrollTop / 11 > 20&&this.flag) {
          this.check = true;
        } else {
          this.check = false;
        }
      },
      backTop() {
        const that = this
        let timer = setInterval(() => {
          let ispeed = Math.floor(-that.scrollTop / 5)
          document.documentElement.scrollTop = document.body.scrollTop = that.scrollTop + ispeed
          if (that.scrollTop === 0) {
            clearInterval(timer)
          }
        }, 16)
      },
      scrollToTop() {
        const that = this
        let scrollTop = window.pageYOffset || document.documentElement.scrollTop || document.body.scrollTop
        that.scrollTop = scrollTop
        if (that.scrollTop > 0) {
          that.btnFlag = true
        } else {
          that.btnFlag = false
        }
      },
      childClose(){
          this.isShowed=false
      },
      childOpen(){
          this.isShowed=true
      },
      reveal(){
        this.check=false;
        this.flag=false
      },
      childLogin(){
        this.login=false
      },
      back(){
        this.login=true
      }
    }
  }
</script>

<style>

</style>