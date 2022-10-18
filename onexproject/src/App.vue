<template>
  <div class="app" :class="mode">
    <div class="head">
      <Header :mode="mode" @toggle="toggle"></Header>
    </div>
    <div class="MainCards">
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

    <div class="OverViewHead">
      <div class="container">
        <div class="row">
          <div class="col-sm-12">
            <OverViewHeader></OverViewHeader>
          </div>
        </div>
      </div>
    </div>

    <div class="OverViewCards1">
      <div class="container">
        <div class="row">
          <div class="col-sm-3">
            <OverviewCards></OverviewCards>
          </div>
          <div class="col-sm-3">
            <OverviewCards></OverviewCards>
          </div>
          <div class="col-sm-3">
            <OverviewCards></OverviewCards>
          </div>
          <div class="col-sm-3">
            <OverviewCards></OverviewCards>
          </div>
        </div>
      </div>

      <div class="OverViewCards2">
        <div class="container">
          <div class="row">
            <div class="col-sm-3">
              <OverviewCards></OverviewCards>
            </div>
            <div class="col-sm-3">
              <OverviewCards></OverviewCards>
            </div>
            <div class="col-sm-3">
              <OverviewCards></OverviewCards>
            </div>
            <div class="col-sm-3">
              <OverviewCards></OverviewCards>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Header from "./Components/Header.vue";
import Cards from "./Components/Cards.vue";
import OverviewCards from "./Components/OverviewCards.vue";
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
    OverviewCards,
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
