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
              :coolrr = "'color:hsl(163, 72%, 41%)'"
              :v="'up'"
              :Color= "'Facebook'"
              :AllTimeFollwer="'1987'"
              :NumberOfFollwersPerDay="12"
              :Following="'Followers'"
              :Srcc= "'icon-facebook'"
            ></Maincards>
          </div>
          <div class="col-sm-3">
            <Maincards
              :coolrr = "'color:hsl(163, 72%, 41%)'"
              :v="'up'"
              :Color= "'Instagram'"
              :AllTimeFollwer="'1044'"
              :NumberOfFollwersPerDay="99"
              :Following="'Followers'"
              :Srcc= "'icon-twitter'"
            ></Maincards>
          </div>
          <div class="col-sm-3">
            <Maincards
              :coolrr = "'color:hsl(163, 72%, 41%)'"
              :v="'up'"
              :Color= "'Twitter'"
              :AllTimeFollwer="'11K'"
              :NumberOfFollwersPerDay="1099"
              :Following="'Followers'"
              :Srcc= "'icon-instagram'"
            ></Maincards>
          </div>
          <div class="col-sm-3">
            <Maincards
              :coolrr = "'color:hsl(356, 69%, 56%)'"
              :v="'down'"
              :Type="Foo"
              :Color= "'Youtube'"
              :AllTimeFollwer="'8239'"
              :NumberOfFollwersPerDay="144"
              :Following="'Subscriber'"
              :Srcc= "'icon-youtube'"
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
              :coolr= "'color:hsl(163, 72%, 41%)'"
              :Val="'up'"
              :src= "'icon-facebook'"
              :Name="'Page Views'"
              :Followers="'87'"
              :Growth="'3'"
            ></OverviewCards>
          </div>
          <div class="col-sm-3">
            <OverviewCards
              :coolr="'color:hsl(356, 69%, 56%)'"
              :Val="'down'"
              :src= "'icon-facebook'"
              :Name="'Likes'"
              :Followers="'52'"
              :Growth="'2'"
            ></OverviewCards>
          </div>

          <div class="col-sm-3">
            <OverviewCards
              :coolr= "'color:hsl(163, 72%, 41%)'"
              :Val="'up'"
               :src= "'icon-instagram'"
              :Name="'Likes'"
              :Followers="'5462'"
              :Growth="'2257'"
            ></OverviewCards>
          </div>

          <div class="col-sm-3">
            <OverviewCards
            :coolr= "'color:hsl(163, 72%, 41%)'"
              :Val="'up'"
              :src= "'icon-instagram'"
              :Name="'Profile Views'"
              :Followers="'52K'"
              :Growth="'1375'"
            ></OverviewCards>
          </div>
        </div>
      </div>

      <div class="OverViewCards2">
        <div class="container">
          <div class="row">
            <div class="col-sm-3">
              <OverviewCards
              :coolr= "'color:hsl(163, 72%, 41%)'"
              :Val="'up'"
              :src= "'icon-twitter'"
              :Name="'Retweets'"
              :Followers="'117'"
              :Growth="'303'"
              ></OverviewCards>
            </div>
            <div class="col-sm-3">
              <OverviewCards
              :coolr= "'color:hsl(163, 72%, 41%)'"
              :Val="'up'"
              :src= "'icon-twitter'"
              :Name="'Likes'"
              :Followers="'507'"
              :Growth="'553'"
              ></OverviewCards>
            </div>

            <div class="col-sm-3">
              <OverviewCards
              :coolr="'color:hsl(356, 69%, 56%)'"
              :Val="'down'"
              :src= "'icon-youtube'"
              :Name="'Likes'"
              :Followers="'107'"
              :Growth="'19'"
              ></OverviewCards>
            </div>

            <div class="col-sm-3">
              <OverviewCards
              :coolr="'color:hsl(356, 69%, 56%)'"
              :Val="'down'"
              :src= "'icon-youtube'"
              :Name="'Total Vies'"
              :Followers="'1407'"
              :Growth="'12'"
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
