<script>
export default {
    name: 'SecondSection',
    methods: {
        getImg(img) {
            return new URL (`../../assets/${img}.png`, import.meta.url).href
        }
    }
}
</script>

<template>
  <section class="position-relative text-center">
    <img :src="getImg('globe1')" alt="">
    <div class="container_custom">
        <h1>anidio quick facts</h1>
        <div class="cards d-flex justify-content-between my-5">
            <div class="card rounded-4">
                <h1>700+</h1>
                <p>Project done</p>
            </div>
            <div class="card rounded-4">
                <h1>250+</h1>
                <p>Happy Clients</p>
            </div>
            <div class="card rounded-4">
                <h1>25+</h1>
                <p>Team Members</p>
            </div>
            <div class="card rounded-4">
                <h1>12+</h1>
                <p>Years on the market</p>
            </div>
        </div>
    </div>
  </section>
</template>

<style lang="scss" scoped>
@use '../../scss/partials/var' as*;
section{
    background-image: url(../../assets/counter-bg.png);
    background-position: center;
    img{
        height: 500px;
    }
    .container_custom{
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translate(-50%,-50%);    
        h1{
        color: $white;
        font-weight: 700;
        font-size: 60px;
        text-transform: capitalize;
        }
        .card{
            width: 220px;
            padding: 20px 0;
            background: none;
            border: 1px solid $white;
            p{
                color: $orange;
            }
        }
    }
}
</style>