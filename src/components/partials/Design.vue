<script>
export default {
    name: 'Design',
    methods: {
        getImg(img) {
            return new URL (`../../assets/${img}.png`, import.meta.url).href
        }
    }

}
</script>

<template>
    
  <div class="d-flex justify-content-between position-relative size">

    <div class="center position-absolute">
        <img :src="getImg('globe3')" alt="">
    </div>

    <div class="left position-relative">
        <img class="dots dots-left" :src="getImg('dots-left')" alt="">        
        <img class="globe-one" :src="getImg('globe1')" alt="">
        <img class="man position-absolute bottom-0" :src="getImg('left-man')" alt="">

    </div>
    <div class="right text-end "> 
        <img class="dots dots-right" :src="getImg('dots-right')" alt="">        
        <img class="light" :src="getImg('light')" alt="">     
        <img class="globe" :src="getImg('globe2')" alt="">     
        <img class="man" :src="getImg('right-man')" alt="">
  
    </div>
  </div>
</template>

<style lang="scss">
.size{
    padding-top: 100px;
}

.dots{
    position: absolute;
}
.dots-left{
    left: 100px;
    top: 50px;
}
.dots-right{
    right: 0;
    top: 70px;
}

.center{
    bottom:600px;
    left: 50%;
    transform: translate(-50%);
}
.man{
    height: 400px;    
}
.globe-one{
    display: block;
    padding-left: 130px;
    margin-top: 50px;
    height: 150px;
}
.globe{
    display: block;
    padding-right: 400px;
    height: 100px;
}
.light{
    padding-right: 130px;
}
</style>