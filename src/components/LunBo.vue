<template>
<div>
    <div class="bigbox">
      <div style="float:left">
            <div class="smallbox">
            <img :src=srcList[currentIndex] :title="titleList[currentIndex]">
            </div>
            <button class="left" @click="gopre">&lt;</button>
            <button class="right" @click="gonex">&gt;</button>
            <ul >
                <li v-for="(item,index) in srcList" :class="index==currentIndex?'active':'inactive'" @mouseover="change(index)" :key="item"></li>
            </ul>
      </div>
     
      </div>
      <div class="bf">
        <span><h2>战地（EA公司发行的第一人称射击游戏系列）</h2> </span><br>
        <span>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;战地系列游戏以大规模的载具和步兵在大地图上协同作战为品牌卖点，注重游戏娱乐性的同时兼顾真实性。战地系列历来是网络游戏，有一些产品同时设计了作为附加模式的单机游戏。部分战地系列游戏的扩展功能比较完善，第三方团体可以制作各种各样的模组满足玩家不同的需要。传统的战地系列游戏主攻PC平台；自2005年起，开发组也逐渐重视起游戏机平台。</span><br><br>
        <span>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;美国艺电只零星地公布过部分战地系列游戏的销量。截止2011年底，战地系列总销量已超过4000万，是历史第2热卖Fps系列。据Metacritic统计，除了免费游戏《战地：英雄》和扩充包《战地2：欧洲力量》，其它战地游戏获得的75分以上的平均评分，其中《战地2》达到了系列中最高的91分，而《战地3》在发售首日便得到了93分评论媒体称赞每一款战地游戏中丰富的载具、合理设计的兵种系统可以让玩家体验高质量的网络对战，同时指出各作品都不同程度地存在单人游戏部分薄弱、程序漏洞较多、游戏优化欠佳的问题。</span>
     </div>
</div>

</template>

<script>
export default {
  name: 'LunBo',
  data :function(){
      return{
            currentIndex:0,
           titleList:["战地3","战地5","战地2042","战地4","战地1"],
           srcList:[require("../assets/img/bf33.jpeg"),require("../assets/img/bf55.jpeg"),require("../assets/img/2042.jpg"),require("../assets/img/bf44.jpeg"),require("../assets/img/bf11.jpeg")]
      }
    },
    methods:{
      gopre:function(){
           if(this.currentIndex==0){
                   this.currentIndex=4
               }else{
                   this.currentIndex--;
               }
            },
      gonex:function(){
            if(this.currentIndex==4){
                   this.currentIndex=0
               }else{
                   this.currentIndex++;
               }
      },
      change:function(index){
        this.currentIndex=index
      }  
    },
  
}
</script>
<style scoped>
@import '../assets/css/home/lunbo.css'
</style>