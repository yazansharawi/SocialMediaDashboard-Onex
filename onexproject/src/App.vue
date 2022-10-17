
<template>
  <div class = 'app' :class = "mode">
    <Header :mode = "mode" @toggle = "toggle"></Header>
</div>
</template>

<script>

import Header from './Components/Header.vue'

export default {
  name: 'App',
  data (){
    return{
      mode: 'light'
    }
  },
  components: {
    Header,
  },
  methods:{
    toggle(){
      if(this.mode === "dark"){
        this.mode = "light";
      }else{
        this.mode = "dark";
      }
    }
  }
}
</script>
<style>
@import './App.css';
</style>
