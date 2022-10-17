
<template>
  <div class = 'app' :class = "mode">
    <Header :mode = "mode"></Header>
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
}
</script>
<style>
@import './App.css';
</style>
