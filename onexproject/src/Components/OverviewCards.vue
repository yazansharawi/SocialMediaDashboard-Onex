<template>
  <div class="cardOverView">
    <div class="container">
        <div class="CardOverViewBody">
          <div class = "PageNamePlusIcon">
            <div>
              <p class = "pagename" >{{Name}}</p>
            </div>
            <div>
              <span><img :src="require(`../assets/${Src}.svg`)" alt=""></span>
            </div>
          </div>
          <div class = "FollowersPlusGrowth">
            <div>
              <p class = "followers" >{{Followers}} </p>
            </div>
            <div>
              <p :style = "coolr" class = "growth"><img :src="require(`../assets/icon-${Val}.svg`)" alt="">{{Growth}}%</p>
            </div>
          </div>
        
    </div>
  </div>
</div>
</template>

<script>
export default {
  name: "OverviewCards",
  props: {
    Name:String,
    Followers:String,
    Growth:String,
    Val:String,
    Src:String,
    coolr:String,
  },
};
</script>

<style>
@import "./OverviewCards.css";
</style>
