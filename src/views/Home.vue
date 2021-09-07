<template>
  <div class="home">
    
    <lun-bo/>
    <div class="dis1">
      <br>
      战地1(2016)——IGN评分9分的完美震撼之作
      <br>
      <button>查看详情</button>
      </div>
    <div style="height: 900px">  
        <img src="../assets/img/bf1.png" style="width:100%">
        <div class="float1">总有一天，这些战事都会结束。
                           <br>   这场能完结所有战争的战争，终将分出胜负。
                           <br>  枪炮都会腐蚀，绿草会再次生长。
                           <br>  届时所有战争的痕迹将不复存在。
                           <br>  这块土地会自己慢慢痊愈，像所有其他的伤痛一样。
                           <br>  到时我们肯定早已入土长眠，但也许尚未被世人遗忘。
                           <br>  只要历史记下了我们之中千分之一的人。
                           <br> 未来就会充满我们的生平事迹与故事。
                           <br>  我们的战斗方式、我们的生活方式、还有我们的死亡方式。
                           <br>  等到一切尘埃落定，而我们赢得了胜利时。
                           <br>  他们将会记住我们。
                           <br>  但直到那天到来前，我们会继续战斗，我们会直视死神。
                           <br>  并且战至最后一刻！
                           <br>                    ----出自battlefield1
          </div>
     </div>
     <foot/>
     <div class="dis2">
       <br>
      战地5(2018)——外挂泛滥，半成品的砸牌屑作？
      <br>
      <button>查看详情</button>
      </div>
   <div style="height:910px">
     <img src="../assets/img/bf5.png" style="width:100%">
     <div class="float2">
            <br>在战地5中见识了800m爆头小左轮、迷彩光学隐身刀客、闪电侠、不死术士之后，我才深刻的体会到战争的恐怖和前人的艰辛，愿世界和平.
            <br>
            <br>这是二战的战场吗，为什么大家都有超能力？
            <br>
            <br>玩了这游戏，对前辈感到佩服与致敬，他们不仅要面对威力巨大的坦克和密集式轰炸的飞机，还要面对各种各样的超人。
            <br> ----出自battlefieldVsteam社区评论
     </div>
   </div>

   
    <div class="dis3">
      <br>
      战地2042(2021)——近未来的混乱战斗
      <br>
      <button>查看详情</button>
    </div>
      
    <div style="height:850px">
     <img src="../assets/img/2042.jpg" style="width:100%">
      <div class="detail">
      
        
      </div>
     <div class="float3">
        <br>《战地风云 2042》游戏背景设定为近未来，会有动态的天气系统，以及改善后的破坏系统。本作为《战地风云》系列首次支持 128 名玩家同时加入全面战争——让玩家有机会参与大规模战斗。
        <br>《战地2042》带领玩家重返该系列标志性的全面战争。走进因失序而面目全非的近未来世界，在小队队友和尖端武器的帮助下，适应并征服瞬息万变的战场。
     </div>
   </div>


      <div class="dis4">
      <br>
      <span style="color:white">前往论坛</span>
      <button>查看详情</button>
      </div>
<div style="height:500px">
  <img src="../assets/img/forum.png" style="width:100%">
  <div class="float4">
    <span>前往战地社区了解更多咨询</span><br><br><br>
    <button>了解更多</button>
    <button class="button" style="z-index:0">点击显示更多内容</button>
  </div>
</div>
  </div>
  <lun-bou/>
</template>

<script>
// @ is an alias to /src
//使用其他组件
import TopNav from '@/components/TopNav.vue'
import LunBo from '@/components/LunBo.vue'
import LunBou from '@/components/LunBou.vue'




export default {
  name: 'Home',
  components: {
    TopNav,
    LunBo,
    LunBou
  }
}
</script>
