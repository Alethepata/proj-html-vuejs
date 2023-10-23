<script>
export default {
    name: 'Video',
    methods: {
        getImg(img) {
            return new URL(`../../assets/${img}.png`, import.meta.url).href
        }
    }
}
</script>

<template>
  <div class="container_custom">
    <div class="video position-relative">
        <img class="w-100 object-fit-cover " :src="getImg('middle')" alt="">
        <i class="fa-solid fa-play play rounded-circle"></i>
    </div>
  </div>
</template>

<style lang="scss">
@use '../../scss/partials/var' as *;
.play{
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%,-50%);
    color: $white;
    font-size: 30px;
    background-color: $magenta;
    text-align: center;
    line-height: 80px;
    height: 80px;
    width: 80px;
    &:hover{
        line-height: 100px;
        height: 100px;
        width: 100px;
    }
}
</style>