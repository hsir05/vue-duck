<template>
<div class="duck-box">
    <div class="duck-container">
        <div class="duck-body"></div>
        <div class="duck-legs"></div>
        <div class="duck-neck"></div>
        <div class="duck-head"></div>
    </div>
</div>
</template>
<script lang="ts" setup>

</script>
<style lang="css" scoped>
.duck-box{
    background-color: #f9f8f8;
}
.duck-container{
    height: 400px;
    width: 400px;
    position: relative;
    margin: 0 auto;
}
.duck-body{
    position: absolute;
    top: 135px;
    height: 120px;
    width: 240px;
    z-index: 1;
    border-radius: 0 0 120px 120px;
    background-color:  #c3d3e4;
}
.duck-body:after{
    content: "";
    height: 20px;
    width: 30px;
    background-color: #998378;
    border-radius: 0 0 0 20px;
    z-index: -1;
    position: absolute;
    left: -26px;
    transform: translateZ(-10px);
}
.duck-legs{
    height: 20px;
    width: 10px;
    background-color: #e9a52a;
    position: absolute;
    top: 255px;
    left: 110px;
}
.duck-legs:after{
    content: "";
    height: 15px;
    width: 30px;
    background-color: #e9a52a;
    border-radius: 0 15px 0 0;
    position: absolute;
    bottom: 0;
}
.duck-neck{
    position: absolute;
    top: 46px;
    left: 235px;
    height: 120px;
    width: 60px;
    border-radius: 0 100px 100px 0;
    background-image: radial-gradient(circle at left center, #f9f8f8, #f9f8f8 33.333%, #88abc3 33.333%, #88abc3 52.666%, #aac3df 6.666%, #aac3df);
}
.duck-head{
    position: absolute;
    top: 32.5px;
    left: 235px;
    overflow: hidden;
    height: 50px;
    width: 150px;
    border-radius: 15px 0 50px;
    background-image: linear-gradient(to right, #c2d7e2, #c2d7e2 25%, #f1c066 25%, #f1c066);
}
.duck-head::after{
    content: "";
     height: 10px;
    width: 10px;
    background-color: #333;
    border-radius: 50%;
    position: absolute;
    top: 20px;
    left: 25%;
    transform: translateX(-50%);
    box-shadow: 0 0 0 5px #6c5a5b;
}
</style>