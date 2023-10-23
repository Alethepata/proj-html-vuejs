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
  <section>
    <div class="container_custom d-flex justify-content-end position-relative">
        <img class="image position-absolute h-100" :src="getImg('process-thumb')" alt="">
        <div class="content">
            <div class="text">
                <h4>our process</h4>
                <h1>our process for your animation production</h1>
                <p class="my-3">We have an effective for working on animation</p>
            </div>
            <div class="cards d-flex justify-content-between">
                <div class="card rounded-4 me-3 position-relative">
                    <div class="number">
                        <p>4</p>
                    </div>
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
                    <div class="number">
                        <p>1</p>
                    </div>
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
            <div class="arrows d-flex ">
                <i class="fa-solid fa-arrow-left me-2"></i>
                <i class="fa-solid fa-arrow-right"></i>
            </div>
        </div>   
    </div>
  </section>
</template>

<style lang="scss" scoped>
@use '../../scss/partials/var' as*;
.image{
    left: -250px;
}
.content{
    width: 50%;
    .card{
        text-align: center;
        padding: 40px 25px;
        .number{
            position: absolute;
            right: 20px;
            top: 0;
            width: 40px;
            background-color: lighten($light-violet, 40%);
            border-bottom-left-radius:50px;
            border-bottom-right-radius:50px;
            p{
                margin-top: 30px;
                margin-bottom: 10px;
            }
        }
        .card-image{
            img{ 
                
                margin-bottom: 20px;  
            }
        }
        .card-text{
            color: $violet;
        }
    }
}

</style>