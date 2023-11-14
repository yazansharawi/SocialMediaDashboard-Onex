<template>
  <header>
    <div class="HeadPage">
      <div class="container">
        <div class="row">
          <div class="col-sm-4">
            <h3 class = "h3MainHead">Social Media Dashboard</h3>
            <h5 class="TotalFollwers">Totol Follwers : 23,004</h5>
          </div>

          <div class="col-sm-5"></div>

          <div class="col-sm-3" id = "but">
            <div class = "ModeName"> <h5>{{ mode }} Mode</h5></div>
            <div>
              <label class="switch">
              <input
                type="checkbox"
                :checked="mode == 'dark' ? 'checked' : false"
                @change="$emit('toggle')"
              />
              <span class="toggle round"></span>
            </label></div>
          </div>
        </div>
      </div>
    </div>
  </header>
</template>

<script>
import Toggle from "./Toggle.vue";
export default {
  props: ["mode"],
  name: "Header",
  components: { Toggle },
};
</script>

<style>
@import "./Header.css";
@import "~bootstrap/dist/css/bootstrap.css";
</style>
