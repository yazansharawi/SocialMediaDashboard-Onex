<template>
    <div class="cardOverView">
      <div class="container">
        <div class="row">
          <div class="CardOverViewBody1">
          <div class="row-sm-6">
              <div class="container">
                <div class="row">
                <div class="col-sm-8">
                  <p>Page Views</p>
                </div>
                <div class="col-sm-4">
                  <i class="fa-brands fa-facebook fa-2xl"></i>
                </div>
              </div>
              </div>
            </div>
          </div>
          <div class="CardOverViewBody2">
          <div class="row-sm-6">
              <div class="container" >
                <div class="row">
                <div class="col-sm-6">
                  <h3>87</h3>
                </div>
                <div class="col-sm-6">
                  <h5>^3%</h5>
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
  name: "Cards",
  props: ["Color", "Img", "AllTimeFollwers", "NumberOfFollwersPerDay"],
  data :function(){

  }
};
</script>

<style>
@import "./OverviewCards.css";
</style>
