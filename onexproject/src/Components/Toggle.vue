<template>
    <div class = "toggle-wrapper">
        <label class = "toggle">
            <input type="checkbox" :checked = "(mode == 'dark') ? 'cheaked' : false">
            <span class = "toggle round"></span>
        </label>
    </div>
</template>

<script>
export default{
    props:['mode']
}
</script>


<style>
@import "./Toggle.css";
</style>