<template>
  <div class="app" :class="mode">
    <div class="head">
      <Header :mode="mode" @toggle="toggle"></Header>
    </div>
    <div class="cards">
      <div class="container">
        <div class="row">
          <div class="col-sm-3">
            <Cards
              :Color="yazan"
              :AllTimeFollwers="3000"
              :NumberOfFollwersPerDay="3000"
              img="uu"
            ></Cards>
          </div>
          <div class="col-sm-3">
            <Cards
              :Color="yazan"
              :AllTimeFollwers="3000"
              :NumberOfFollwersPerDay="3000"
              img="uu"
            ></Cards>
          </div>
          <div class="col-sm-3">
            <Cards
              :Color="yazan"
              :AllTimeFollwers="3000"
              :NumberOfFollwersPerDay="3000"
              img="uu"
            ></Cards>
          </div>
          <div class="col-sm-3">
            <Cards
              :Color="yazan"
              :AllTimeFollwers="3000"
              :NumberOfFollwersPerDay="3000"
              img="uu"
            ></Cards>
          </div>
        </div>
      </div>
    </div>
    <div class="container">
      <div class="row">
        <div class="col-sm-12">
          <OverViewHeader></OverViewHeader>
        </div>
      </div>
    </div>
    <div class="container">
      <div class="row">
        <div class="col-sm-3">
          <Overview1></Overview1>
        </div>
        <div class="col-sm-3">
          <Overview1></Overview1>
        </div>
        <div class="col-sm-3">
          <Overview1></Overview1>
        </div>
        <div class="col-sm-3">
          <Overview1></Overview1>
        </div>
      </div>
    </div>
    <div class="container">
      <div class="row">
        <div class="col-sm-3">
          <Overview1></Overview1>
        </div>
        <div class="col-sm-3">
          <Overview1></Overview1>
        </div>
        <div class="col-sm-3">
          <Overview1></Overview1>
        </div>
        <div class="col-sm-3">
          <Overview1></Overview1>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Header from "./Components/Header.vue";
import Cards from "./Components/Cards.vue";
import Overview1 from "./Components/Overview1.vue";
import OverViewHeader from "./Components/OverViewHeader.vue";

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
    Overview1,
    OverViewHeader,
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
