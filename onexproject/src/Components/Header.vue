<template>
    <div class="HeadPage">
    <div class="container">
  <div class="row">
    <div class="col-sm-4">
      <h3>Social Media Dashboard</h3>
      <h5>Totol Follwers : 23,004</h5>
    </div>
    <div class="col-sm-4">

    </div>
    <div class="col-sm-4">
        <h1>{{mode}} Mode</h1>
    </div>
  </div>
</div>
</div>
</template>


<script>
export default{
    props:['mode'],
    name: "Header",
    components: {},
}
</script>

<style>
@import './Header.css';
@import'~bootstrap/dist/css/bootstrap.css'

</style>