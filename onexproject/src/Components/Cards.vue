<template>
  <div class="container">
    <div class="row">
      <div class = card1>
      <div class="card text-center">
        <div class="card-body">
          <h5 class="card-title">{{Color}}</h5>
          <p class="card-text">
            {{AllTimeFollwers}}
          </p>
          <p class="card-text">
            {{NumberOfFollwersPerDay}}
          </p>
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
