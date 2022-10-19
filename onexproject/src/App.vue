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
              :Color= "'Facebook'"
              :AllTimeFollwer="'1987'"
              :NumberOfFollwersPerDay="12"
              :Following="'Followers'"
              :val="'fa-brands fa-square-facebook fa-2xl'"
            ></Maincards>
          </div>
          <div class="col-sm-3">
            <Maincards
            :Color= "'Instagram'"
              :AllTimeFollwer="'1044'"
              :NumberOfFollwersPerDay="99"
              :Following="'Followers'"
              :val="'fa-brands fa-square-instagram fa-2xl'"
            ></Maincards>
          </div>
          <div class="col-sm-3">
            <Maincards
            :Type="Foo"
            :Color= "'Twitter'"
              :AllTimeFollwer="'11K'"
              :NumberOfFollwersPerDay="1099"
              :Following="'Followers'"
              :val="'fa-brands fa-square-twitter fa-2xl'"
            ></Maincards>
          </div>
          <div class="col-sm-3">
            <Maincards
              :Type="Foo"
              :Color= "'Youtube'"
              :AllTimeFollwer="'8239'"
              :NumberOfFollwersPerDay="144"
              :Following="'Subscriber'"
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
            :Name="'Page Views'"
              :Val="'fa-brands fa-square-facebook fa-2xl'"
              :Followers="'87'"
              :Growth="'3'"
            ></OverviewCards>
          </div>
          <div class="col-sm-3">
            <OverviewCards
            :Name="'Likes'"
              :Val="'fa-brands fa-square-facebook fa-2xl'"
              :Followers="'52'"
              :Growth="'2'"
            ></OverviewCards>
          </div>

          <div class="col-sm-3">
            <OverviewCards
            :Name="'Likes'"
              :Val="'fa-brands fa-square-instagram fa-2xl'"
              :Followers="'5462'"
              :Growth="'2257'"
            ></OverviewCards>
          </div>

          <div class="col-sm-3">
            <OverviewCards
            :Name="'Profile Views'"
              :Val="'fa-brands fa-square-instagram fa-2xl'"
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
              :Name="'Retweets'"
              :Val="'fa-brands fa-square-facebook fa-2xl'"
              :Followers="'117'"
              :Growth="'303'"
              ></OverviewCards>
            </div>
            <div class="col-sm-3">
              <OverviewCards
              :Name="'Likes'"
              :Val="'fa-brands fa-square-facebook fa-2xl'"
              :Followers="'507'"
              :Growth="'553'"
              ></OverviewCards>
            </div>

            <div class="col-sm-3">
              <OverviewCards
              :Name="'Likes'"
              :Val="'fa-brands fa-square-facebook fa-2xl'"
              :Followers="'107'"
              :Growth="'19'"
              ></OverviewCards>
            </div>

            <div class="col-sm-3">
              <OverviewCards
              :Name="'Total Vies'"
              :Val="'fa-brands fa-square-facebook fa-2xl'"
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
