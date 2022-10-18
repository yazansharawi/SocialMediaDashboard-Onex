<template>
  <div class="app" :class="mode">
    <div class="head">
      <Header :mode="mode" @toggle="toggle"></Header>
    </div>
    <div class="mainCards">
      <div class="container">
        <div class="row">
          <div class="col-sm-3">
            <Maincards
              :Color="yazan"
              :AllTimeFollwer="3010"
              :NumberOfFollwersPerDay="3100"
              :fathi="'Followers'"
              :val="'fa-brands fa-square-facebook fa-2xl'"
            ></Maincards>
          </div>
          <div class="col-sm-3">
            <Maincards
              :Color=yazan
              :AllTimeFollwer="3000"
              :NumberOfFollwersPerDay="3000"
              :fathi="'Followers'"
              :val="'fa-brands fa-square-instagram fa-2xl'"
            ></Maincards>
          </div>
          <div class="col-sm-3">
            <Maincards
            :Type="Foo"
              :Color="yazan"
              :AllTimeFollwer="3000"
              :NumberOfFollwersPerDay="3000"
              :fathi="'Followers'"
              :val="'fa-brands fa-square-twitter fa-2xl'"
            ></Maincards>
          </div>
          <div class="col-sm-3">
            <Maincards
              :Type="Foo"
              :Color="yazan"
              :AllTimeFollwer="3000"
              :NumberOfFollwersPerDay="3000"
              :fathi="'Subscriber'"
              :val="'fa-brands fa-square-youtube fa-2xl'"
            ></Maincards>
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
            <OverviewCards
              :PageName="Likes"
              :color="green"
              :NumbersOfLikes="33"
              :NumbersOfGrowth="34"
            ></OverviewCards>
          </div>
          <div class="col-sm-3">
            <OverviewCards
              :PageName="Likes"
              :color="green"
              :NumbersOfLikes="33"
              :NumbersOfGrowth="34"
            ></OverviewCards>
          </div>

          <div class="col-sm-3">
            <OverviewCards
              :PageName="Likes"
              :color="green"
              :NumbersOfLikes="33"
              :NumbersOfGrowth="34"
            ></OverviewCards>
          </div>

          <div class="col-sm-3">
            <OverviewCards
              :PageName="Likes"
              :color="green"
              :NumbersOfLikes="33"
              :NumbersOfGrowth="34"
            ></OverviewCards>
          </div>
        </div>
      </div>

      <div class="OverViewCards2">
        <div class="container">
          <div class="row">
            <div class="col-sm-3">
              <OverviewCards
                :PageName="yazan"
                :color="green"
                :NumbersOfLikes="33"
                :NumbersOfGrowth="34"
              ></OverviewCards>
            </div>
            <div class="col-sm-3">
              <OverviewCards
                :PageName="Likes"
                :color="green"
                :NumbersOfLikes="33"
                :NumbersOfGrowth="34"
              ></OverviewCards>
            </div>
            <div class="col-sm-3">
              <OverviewCards
                :PageName="Likes"
                :color="green"
                :NumbersOfLikes="33"
                :NumbersOfGrowth="34"
              ></OverviewCards>
            </div>
            <div class="col-sm-3">
              <OverviewCards
                :PageName="Likes"
                :color="green"
                :NumbersOfLikes="33"
                :NumbersOfGrowth="34"
              ></OverviewCards>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Header from "./Components/Header.vue";
import Maincards from "./Components/Maincards.vue";
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
    Maincards,
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
