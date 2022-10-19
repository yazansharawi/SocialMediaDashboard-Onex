<template>
  <div class="CardsMargin">
    <div class="container">
      <div class="row">
        <div class="card1" data-color="blue" v-bind:class=Color >
          <div class="col-sm-12">
            <div class="Name">
              <div class="UserName" >
                <div> <i :class = "val"></i></div>
                <div><a href="https://www.instagram.com/yazan_sharawi_/">Yazan Sharawi</a></div>
              </div>
            </div>

            <div class="AllTimeFollwers">
              <p class="NumOfFollwers">{{ AllTimeFollwer }}</p>
              <p class = "FollowersMain">{{ Following }}</p>
            </div>
            
            <div class="FollwersPerDay">
              <p class = "GrowthMain" style="color:hsl(163, 72%, 41%)" > ^{{ NumberOfFollwersPerDay }} Today</p>
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
  },
};
</script>

<style>
@import "./Maincards.css";
</style>
