<template>
<div>
    <div class="sideNav" style="z-index:100">
            <h2>aboutBATTLEFIELD</h2><span class="closebtn" @click="closeit"></span>
            <h5>了解战地风云系列的前世今生</h5>
     
        <h3><router-link to="/games">历代游戏</router-link> </h3> <br>
       
         <h3><a href="https://baike.baidu.com/item/DICE/7456761?fr=aladdin" target="new">开发商</a></h3> <br>
        
       
          <h3><a href="https://baike.baidu.com/item/%E5%AF%92%E9%9C%9C%E5%BC%95%E6%93%8E/8391328?fr=aladdin" target="new">寒霜引擎</a></h3><br>
       
       
         <h3><a href="https://answers.ea.com/t5/Battlefield/ct-p/battlefield" target="new">论坛</a></h3> <br>
     
        <h4>有建议？请联系：2276001806@qq.com</h4>
    </div>
    
</div>
</template>

<script>
export default {
  name: 'SideNav',
  data :function(){
      return{
          isShowed:true,
          childBlock:false
      }
    },
    methods:{
      closeit:function(){
            this.$emit('parentClose',this.isShowed,this.childBlock)
      }
    },
  
}
</script>

<style>

</style>