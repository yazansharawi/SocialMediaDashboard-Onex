<template>
  <div class = "CardsMargin">
  <div class="container">
    <div class="row">
      <div class = card1>
        <div class="col-sm-12">
        <div class = "CardUpperColor">
        </div>
        <div class = "Name">
          <div class = "UserName">
            <a href="https://www.instagram.com/yazan_sharawi_/" target="_blank" rel="noopener noreferrer"><img src="src/assets/icon-instagram.svg" alt="insta_pic">yazan_sharawi_</a>
          </div>
        </div>
        <div class = "AllTimeFollwers">
          <p class = "NumOfFollwers">11K</p>
          <p>FOLLOWERS</p>
        </div>
        <div class = "FollwersPerDay">
          <p>^ 1099 Today</p>
        </div>
      </div>
    </div>
  </div>
  </div>
</div>
</template>

<script>
export default {
  name: "Cards",
  props:[
    "Color","Img","AllTimeFollwers","NumberOfFollwersPerDay"
  ]
};
</script>

<style>
@import "./Cards.css";
</style>