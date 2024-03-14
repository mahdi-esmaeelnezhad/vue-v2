<template>
  <div class="card">
    <p :style="{color : color}">{{ message }}</p>
    <button @click="clickBtn">{{ textButton }}</button>
  </div>
</template>

<script>

export default{
    name : "CardShow",
    props : {
        message : String,
        colorBtn : String
    },
    data(){
      return{
        textButton : "add",
        color : "red"
      }
    },
    methods : {
        clickBtn : function()
        {
          this.color = this.colorBtn
        },
        clickHandler : function(){

        }
    },
    mounted(){
        console.log("mahdiCard")
    },
    beforeUpdate(){
        console.log("mahdiCard1")
    },
    updated(){
        console.log("mahdiCard2")
    }
}
</script>
  
<style>
  .card{
    background-color: aqua;
  }
</style>
