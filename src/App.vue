<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld msg="Welcome to Your Vue.js App"/>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import jsonp from "jsonp"

export default {
  name: 'App',
  components: {
    HelloWorld
  },
  data(){
    return{
      age:30,
    }
  },
  mounted(){
    let url = "https://www.easy-mock.com/mock/5f6f0151d94dae3ef99d173b/table/list"
    jsonp(url, ()=>{

    })
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
