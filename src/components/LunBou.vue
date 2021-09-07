<template>
<div>
    <div class="bigbox2">
     
            <div class="smallbox2">
            <img id="photo1"  src="../assets/img/bf4.jpg" >
            </div>
            <div class="smallbox2"><img   src="../assets/img/bfV.jpg" alt=""></div>
            <div  class="smallbox2"><img  src="../assets/img/bf3.jpeg" alt=""></div>
            <div class="smallbox2"><img  src="../assets/img/bf2.jpeg" alt=""></div>
            <div class="smallbox2"><img src="../assets/img/bf2042.jpeg" alt=""></div>
            <div class="smallbox2"><img  src="../assets/img/2142.jpeg" alt=""></div>
            <div class="smallbox2"><img  src="../assets/img/1942.jpeg" alt=""></div>
             <div class="smallbox2"><img  src="../assets/img/bad.jpeg" alt=""></div>
    </div>
</div>

</template>

<script>
export default {
  name: 'LunBou',
  data :function(){
      return{
            currentIndex:1,
           srcList:["../assets/img/09.png","../assets/img/10.png","../assets/img/11.png"]
      }
    },
    methods:{
      gopre:function(){
           if(this.currentIndex==0){
                   this.currentIndex=2
               }else{
                   this.currentIndex--;
               }
            },
      gonex:function(){
            if(this.currentIndex==2){
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