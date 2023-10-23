<script>
export default {
    name: 'FourthSection',
    methods: {
        getImg(img) {
            return new URL (`../../assets/${img}.png`, import.meta.url).href
        }
    }
}
</script>

<template>
  <section class="position-relative">
    <div class="container_custom d-flex position-absolute">
        <img class="image" :src="getImg('process-thumb')" alt="">
        <div class="content ms-5">
            <div class="text">
                <h3>our process</h3>
                <h1>our process for your animation production</h1>
                <p>we have an effective for working on animation</p>
            </div>
            <div class="cards d-flex justify-content-between">
                <div class="card rounded-4 me-2">
                    <div class="card-image">
                        <img :src="getImg('process2')" alt="">
                    </div>
                    <div class="card-text">
                        <h3>Pre-production</h3>
                        <p>
                                We'll take your idea and create a technical script which consists of action notes and animation descriptions

                        </p>
                    </div>
                </div>
                <div class="card rounded-4">
                    <div class="card-image h-100">
                        <img :src="getImg('process1')" alt="">
                    </div>
                    <div class="card-text">
                        <h3>Pre-production</h3>
                        <p>
                                We'll take your idea and create a technical script which consists of action notes and animation descriptions

                        </p>
                    </div>
                </div>
            </div>
        </div>
    </div>
  </section>
</template>

<style lang="scss" scoped>
@use '../../scss/partials/var' as*;
.image{
    
}
.container_custom{
    left: -250px;
}
.card{
    width: 250px;
    text-align: center;
    padding: 25px 10px 20px 10px;
    .card-image{


        img{
            width: 60px;
        }
    }

    .card-text{
        color: $violet;
    }
}
</style>