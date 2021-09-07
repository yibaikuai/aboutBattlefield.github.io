<template >
  <div class="nav" >
    <ul class="topNav">
      <li>
        <a href="javascript:void(0)"
          ><img src="..\assets\img\ea.png" style="height: 50px"
        /></a>
      </li>
      <li>
        <a href="javascript:void(0)"
          ><svg style="margin-top:5px;margin-left:4px" t="1629450184076" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="3792" width="39" height="39 "><path d="M511.001 707.986c-12.817 0-25.566 5.264-34.658 14.355-9.058 9.092-14.355 21.807-14.355 34.658s5.298 25.565 14.355 34.657c9.057 9.092 21.807 14.355 34.658 14.355 12.852 0 25.567-5.264 34.659-14.355s14.355-21.806 14.355-34.657-5.264-25.566-14.355-34.658c-9.057-9.091-21.806-14.355-34.659-14.355zM510.353 234.324c-47.578 0-86.031 15.449-115.356 46.279-29.292 30.864-46.382 73.384-47.305 112.554-0.957 39.204 77.143 31.069 80.014 11.724 3.076-20.507 15.86-53.628 30.762-68.598 14.936-15.005 33.496-22.525 55.678-22.525 23.037 0 41.29 7.212 54.894 21.602 13.603 14.424 20.439 31.719 20.439 51.919 0 14.561-3.896 27.891-11.484 39.99-4.991 7.656-20.235 23.789-45.665 48.501-25.395 24.678-42.417 46.895-50.893 66.582-8.442 19.756-12.715 44.912-12.715 75.537 0 2.939 0.068 11.211 0.307 24.814h79.16c-0.409-28.643 1.642-48.535 6.085-59.609 4.442-11.143 15.858-25.84 34.248-44.023 35.547-35.308 58.72-63.232 69.59-83.672 10.801-20.439 16.27-42.212 16.27-65.146 0-41.46-14.767-77.827-44.435-109.033-29.668-31.24-69.452-46.895-119.526-46.895h-0.068z" fill="#BCBCBB" p-id="3793"></path><path d="M511.001 22c-270.087 0-490 219.81-490 490 0 270.293 219.844 490 490 490s490-219.707 490-490c0.001-270.19-219.775-490-490-490z m-0.307 917.725c-236.25 0-428.339-192.158-428.339-428.237 0-236.25 192.124-428.339 428.339-428.339 236.216 0 428.374 192.055 428.374 428.339 0.068 236.078-192.089 428.237-428.374 428.237z" fill="#BCBCBB" p-id="3794"></path></svg></a>
      </li>
      <li>
        <router-link to="/Login" @click="goLogin">
          <svg  id="user" style="width:44px;height:44px"  t="1629449609393" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="1212"><path d="M512 98.2c63 0 121.5 13.5 175.5 36s103.5 54 144 94.5 72 85.5 94.5 139.5 36 112.5 36 175.5-13.5 121.5-36 175.5-54 99-94.5 139.5-85.5 72-144 94.5c-54 22.5-112.5 36-175.5 36s-121.5-13.5-175.5-36-103.5-54-144-94.5-72-85.5-94.5-139.5-36-112.5-36-175.5 13.5-121.5 36-175.5 54-103.5 94.5-139.5c40.5-40.5 90-72 144-94.5 54-27 112.5-36 175.5-36z" fill="#707070" p-id="1213"></path><path d="M651.44604445 402.4104c0 76.21594075-61.77374815 138.11105185-138.11105186 138.11105186s-138.11105185-61.77374815-138.11105184-138.11105186c0-76.21594075 61.77374815-138.11105185 138.11105184-138.11105184s138.11105185 61.77374815 138.11105186 138.11105184z m-9.46631112 145.15010371c-36.28752592 28.64165925-81.31318518 44.54020741-128.52337778 44.5402074-47.81700741 0-93.20675555-16.26263703-129.7370074-45.5111111-96.24082963 35.31662222-139.20331852 158.62139259-139.20331852 214.93380741h534.84657778c0.12136297-55.82696297-43.20521482-178.16082963-137.38287408-213.96290371z m0 0" fill="#ffffff" p-id="1214"></path></svg></router-link>
      </li>
    </ul>
    <ul class="bottomNav">
      <router-link to="/"  @click="mainweb">
      <li style="text-align:right;width:50px;margin-left:40px" >about</li>
      <li style="width:250px"><img src="../assets/img/logo1.png"/></li>
      </router-link>
      
        
      <li id="container"><router-link to="/Games" @click="mainweb" @mouseenter="lineShow1" @mouseleave="lineUnshow1">历代游戏</router-link>

          <ul v-if="false">
            <div >
           
              <li ><router-link to="/about">战地5</router-link></li>
              <li ><router-link to="/about">战地3</router-link></li>
              <li><router-link to="/about">战地4</router-link></li>
              <li ><router-link to="/about">战地2</router-link></li>
              <li><router-link to="/about">战地1942</router-link></li>
              <li ><router-link to="/about">战地2042</router-link></li>
              <li ><router-link to="/about">战地2142</router-link></li>
            </div>
          </ul>
     
      </li>

      <li><a href="https://baike.baidu.com/item/DICE/7456761?fr=aladdin" target="new" @click="mainweb" @mouseenter="lineShow2" @mouseleave="lineUnshow2">开发商</a></li>
      <li><a href="https://baike.baidu.com/item/%E5%AF%92%E9%9C%9C%E5%BC%95%E6%93%8E/8391328?fr=aladdin" target="new" @click="mainweb" @mouseenter="lineShow3" @mouseleave="lineUnshow3">寒霜引擎</a></li>
      <li><a href="https://answers.ea.com/t5/Battlefield/ct-p/battlefield" @click="mainweb" target="new" style="position:absolute;right:100px">官方论坛</a></li>
      <div class="line1" :class="line1==true?'line1':'none'"></div>
      <div class="line2" :class="line2==true?'line2':'none'"></div>
      <div class="line3" :class="line3==true?'line3':'none'"></div>
    </ul>
      <div class="other" @click="openit"></div>
      
  </div>
</template>

<script>
export default {
  name: 'TopNav',
  data:function(){
    return{
          isShowed:true,
          childBlock:false,
          login:false,
          line1:false,
          line2:false,
          line3:false
      }
  },
  
  methods:{
  
  openit:function(){
    this.$emit('parentOpen',this.isShowed,this.childBlock)
  },
  goLogin:function(){
    this.$emit('parentLogin',this.login)
  },
  mainweb(){
    this.$emit('notLogin')
  },
  lineShow1(){
    this.line1=true;
  },
  lineUnshow1(){
    this.line1=false;
  },
  lineShow2(){
    this.line2=true;
  },
  lineUnshow2(){
    this.line2=false;
  },
  lineShow3(){
    this.line3=true;
  },
  lineUnshow3(){
    this.line3=false;
  }
  }
  

}


</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
@import '../assets/css/nav/topNav.css';
@import '../assets/css/nav/bottomNav.css';
@import '../assets/css/nav/float.css';
@import '../assets/css/home/dis.css';
@import '../assets/css/home/2042.css';
@import '../assets/css/foot/foot.css';
@import '../assets/css/foot/footnav.css';
@import '../assets/css/nav/container.css';
@import '../assets/css/home/backTop.css';
@import '../assets/css/home/sideNav.css';
</style>
