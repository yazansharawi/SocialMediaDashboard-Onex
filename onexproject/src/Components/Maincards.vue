<template>
  <div class="CardsMargin">
    <div class="container">
      <div class="row">
        <div class="card1">
          <div class="col-sm-12">
            <div class="Name">
              <div class="UserName">
                <a
                  href="https://www.instagram.com/yazan_sharawi_/"
                  target="_blank"
                  rel="noopener noreferrer"
                  ><i :class = "val"></i
                  >yazan_sharawi_</a>
              </div>
            </div>
            <div class="AllTimeFollwers">
              <p class="NumOfFollwers">{{ AllTimeFollwer }}K</p>
              <p>{{ fathi }}</p>
            </div>
            <div class="FollwersPerDay">
              <p>^ {{ NumberOfFollwersPerDay }} Today</p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>

export default {
  name: "Maincards",
  props: {
    Color:String,
    AllTimeFollwer:String,
    fathi:String,
    NumberOfFollwersPerDay:String,
    val:String,
  },
};
</script>

<style>
@import "./Maincards.css";
</style>
