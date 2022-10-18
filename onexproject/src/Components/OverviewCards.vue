<template>
  <div class="cardOverView">
    <div class="container">
        <div class="CardOverViewBody">
          <div class="row">
          <div class="col-sm-12">
          <div class="container">
            <div class="row">
              <div class="col-sm-6">
                <div class = "PageViews">
                  <p class = "PageViewsFontSize">Yazan</p>
                </div>

                <div class = "NumberOfViews">
                  <p class = "NumberOfViewsFontSize">{{NumbersOfLikes}}</p>
                </div>
              </div>
              
               <div class="col-sm-6">
                <div class = "Icon">
                  <i class="fa-brands fa-square-facebook fa-2xl"></i>
                </div>
                
                <div class = "NumberOfGrowth">
                  <p class = "NumberOfGrowthFontSize">{{NumbersOfGrowth}}</p>
                </div>
              </div>
        </div>
      </div>
    </div>
      </div>
    </div>
  </div>
</div>
</template>

<script>
export default {
  name: "OverviewCards",
  props:["NumbersOfLikes","color","NumbersOfGrowth"]
};
</script>

<style>
@import "./OverviewCards.css";
</style>
