<template>
  <div>
    <div class="cardOverView">
      <div class="container">
        <div class="row">
          <div class="row-sm-6">
            <div class="CardOverViewBody1">
              <div class="container" style="background-color: green">
                <div class="row">
                <div class="col-sm-6">
                  <p>hello</p>
                </div>
                <div class="col-sm-6">
                  <p>hello1</p>
                </div>
              </div>
              </div>
            </div>
          </div>
          <div class="row-sm-6">
            <div class="CardOverViewBody1">
              <div class="container" style="background-color: red">
                <div class="row">
                <div class="col-sm-6">
                  <p>hello</p>
                </div>
                <div class="col-sm-6">
                  <p>hello1</p>
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
  name: "Cards",
  props: ["Color", "Img", "AllTimeFollwers", "NumberOfFollwersPerDay"],
};
</script>

<style>
@import "./OverviewCards.css";
</style>
