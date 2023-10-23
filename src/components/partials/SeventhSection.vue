<script>
export default {
    name:'SeventhSection',
    methods: {
        getImg(img) {
            return new URL (`../../assets/${img}.png`, import.meta.url).href
        }
    }
}
</script>

<template>
  <section class="position-relative">
    <img class="shape-top" :src="getImg('shape-top')" alt="">
    <div class="container_custom text-center py-5">
      <div class="text">
        <h4>we create new worlds!</h4>
        <h1>want tips on your storytellyng?</h1>
        <p>
          Join our newsletter for tips on how to elevate your brand through storytellyng
        </p>
      </div>
      <div class="email d-flex">
        <input type="email" class="form-control" placeholder="Enter you email">
        <button class="btn_custom_pink">Submit</button>
      </div>
    </div>
    <img class="w-100 h-100 object-fit-contain " :src="getImg('shape-bottom')" alt="">
  </section>
</template>

<style lang="scss" scoped>
@use '../../scss/partials/var' as*;

section{
  background-image: url(../../assets/counter-bg.png);
  background-position: center;
  .shape-top{
        position: absolute;
        left: 0;
        top: 0;
        width: 100%;
        height: 5%;  
    }
  .container_custom{
    width: 60%;
    h1,
    p{
      color: $white;
    }
    h4{
      color: $orange;
    }
    .email{
      background-color: $white;
      padding: 10px;
      border-radius: 50px;
      input{
        border: 0;
        background: none;
      }
      .btn_custom_pink:hover{
          background: $orange;
          border-color: $orange;
          color: $white;
      }
    }
  }
}
</style>