<template>
  <div class="cardOverView">
    <div class="container">
        <div class="CardOverViewBody">
          <div class = "PageNamePlusIcon">
            <div>
              <p class = "pagename" >{{Name}}</p>
            </div>
            <div>
              <i :class = "Val"></i>
            </div>
          </div>
          <div class = "FollowersPlusGrowth">
            <div>
              <p class = "followers">{{Followers}}</p>
            </div>
            <div>
              <p  style="color:hsl(163, 72%, 41%)" class = "growth">^{{Growth}}%</p>
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
  },
};
</script>

<style>
@import "./OverviewCards.css";
</style>
