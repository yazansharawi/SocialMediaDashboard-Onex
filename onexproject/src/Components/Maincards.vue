<template>
  <div class="CardsMargin">
    <div class="container">
      <div class="row">
        <div class="card1" v-bind:class=Color >
          <div class="col-sm-12">
            <div class="Name">
              <div class="UserName" >
                <div> <img :src="require(`../assets/${Srcc}.svg`)" alt=""></div>
                <div class = "NamePlusLogo">@nathanf</div>
              </div>
            </div>

            <div class="AllTimeFollwers">
              <p class="NumOfFollwers">{{ AllTimeFollwer }}</p>
              <p class = "FollowersMain">{{ Following }}</p>
            </div>
            
            <div class="FollwersPerDay">
              <p class = "GrowthMain" :style = "coolrr" > <img :src="require(`../assets/icon-${V}.svg`)" alt="">{{ NumberOfFollwersPerDay }} Today</p>

            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
const colorFromScriptSetup = "'Color'"
</script>

<script>

export default {
  name: "Maincards",
  props: {
    Color:String,
    AllTimeFollwer:String,
    Following:String,
    NumberOfFollwersPerDay:String,
    val:String,
    coolrr:String,
    V:String,
    Srcc:String,
  },
};
</script>

<style>
@import "./Maincards.css";
</style>
