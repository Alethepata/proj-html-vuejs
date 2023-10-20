<script>
export default {
    name:'Design'

}
</script>

<template>
    
  <div class="d-flex justify-content-between position-relative size">

    <div class="center position-absolute">
        <img src="../../assets/globe3.png" alt="">
    </div>

    <div class="left position-relative">
        <img class="dots dots-left" src="../../assets/dots-left.png" alt="">        
        <img class="globe-one" src="../../assets/globe1.png" alt="">
        <img class="man position-absolute bottom-0" src="../../assets/left-man.png" alt="">

    </div>
    <div class="right text-end "> 
        <img class="dots dots-right" src="../../assets/dots-right.png" alt="">        
        <img class="ligth" src="../../assets/light.png" alt="">     
        <img class="globe" src="../../assets/globe2.png" alt="">     
        <img class="man" src="../../assets/right-man.png" alt="">
  
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
.ligth{
    padding-right: 130px;
}
</style>