<template>
  <div id="app">  
    <CardShow color="white" message="this is test"></CardShow>
    <BtnCard @changeEmitHandlerFunc="changeEmit($event)" :EverClickHandler="clickHandlers"></BtnCard>
    <button @click="clickAppHandler" >{{ clickApp }}</button>
  </div>
  
</template>

<script>
import CardShow from './components/ShowCard'
import BtnCard from './components/Button'

export default {
  name: 'App',
  components: {    
    CardShow,
    BtnCard
  },
  data(){
    return{
      clickApp : "click app"
    }
  },
  methods:{
    clickAppHandler : function(){
      this.clickApp  = "app"
    },
    clickHandlers : function(){
      alert("mahdi")
    },
    changeEmit:function(data){
      console.log(data)
    }  
  },
  beforeUpdate(){
    console.log("mahdiapp")
  },
  updated(){
    console.log("mahdiapp2")
  }
}
</script>
 
<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
