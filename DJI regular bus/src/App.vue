<template>
  <div id="app">
<div class="tabs">
  <div class="tab" @click="toggleTab('people');changeColor()" :class="{active:isActive}"><a>人员班车</a></div>
   <div class="tab" @click="toggleTab('pack');changeColor()" :class="{active1:isActive1}"><a>货物班车</a></div>
</div>
<people :is="current" keep-alive></people>
  </div>
</template>

<script>
import people from './components/people'
import pack from './components/pack'

export default{
  name: 'app',
  data () {
    return {
      current:'people',
    isActive:true,
    isActive1:false
    }
  },
  components:{
    people,
    pack
  },
  methods:{
    toggleTab(tab){
      this.current = tab;
    },
    changeColor(){
    this.isActive = !this.isActive;
    this.isActive1 = !this.isActive1;
    }
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
.tab{
  display: inline-block;
 padding: 20px 150px 20px;
 text-align: center;
}
.active{
  background-color: #2eaced;
}
.active1{
  background-color: #2eaced;
}
.tabs{
  display: inline-block;
  border:1px solid grey;
}
</style>
