<template>
<div>
  <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld msg="Welcome to Your Vue.js App"/>
  <h1>Its me</h1>
  <UiGrid/> 
  <div>
    <label>Constant directely exported to main comp</label>
    <input v-model='myexport'/></div>
  <div>
    <label>declared Constant exported and used here.</label><input v-model='sree'/></div></div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

import {bestMovieSeriess,greeting,exportdirectconstant,UiGrid } from './components/Computedproperty.vue'
export default {
  name: 'App',
  components: {
    UiGrid ,HelloWorld
  },
  data(){
    return{
       myexport: bestMovieSeriess,
       sree:exportdirectconstant
       
    }
  }
}

//this method is implemented in computedproperty component
greeting('helo','pradeep');

// once defined that must be exported or used with in the methods used in that component otherwise 
// we cannot use it,,,
// function subtract() {
// 	console.log('werwe');
// }


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
