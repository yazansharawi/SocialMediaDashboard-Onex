<template>
  <div class="app" :class="mode">
    <div class="head">
      <Header :mode="mode" @toggle="toggle"></Header>
    </div>
    <div class="cards">
      <div class="container">
        <div class="row">
          <div class="col">
            <Cards :Color="yazan" :AllTimeFollwers="3000" :NumberOfFollwersPerDay="3000" img="uu"></Cards>
          </div>
          <div  class="col">
            <Cards :Color="yazan" :AllTimeFollwers="3000" :NumberOfFollwersPerDay="3000" img="uu"></Cards>
          </div>
          <div  class="col">
            <Cards :Color="yazan" :AllTimeFollwers="3000" :NumberOfFollwersPerDay="3000" img="uu"></Cards>
          </div>
          <div  class="col">
            <Cards :Color="yazan" :AllTimeFollwers="3000" :NumberOfFollwersPerDay="3000" img="uu"></Cards>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Header from "./Components/Header.vue";
import Cards from "./Components/Cards.vue";

export default {
  name: "App",
  data() {
    return {
      mode: "light",
    };
  },
  components: {
    Header,
    Cards,
  },
  methods: {
    toggle() {
      if (this.mode === "dark") {
        this.mode = "light";
      } else {
        this.mode = "dark";
      }
    },
  },
};
</script>
<style>
@import "./App.css";
</style>
