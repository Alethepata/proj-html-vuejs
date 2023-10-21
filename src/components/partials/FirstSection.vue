<script>
export default {
    name: 'FirstSection',
    methods: {
        getImg(img) {
            return new URL (`../../assets/${img}.png`, import.meta.url).href
        }
    }
}
</script>

<template>
  <section class="d-flex position-relative">
    
    <img class="image one" :src="getImg('smart')" alt=""> 

    <div class="container_custom">

        <div class="text text-center w-75 ">

            <h3>our love for animation</h3>
            <h1>we're storytelling expert with creative smarts</h1>
            <p>
                Our culture inspiries the creative and inovation spirit found throughout our Studio. We breathe life into new ideas!
            </p>

        </div>

        <div class="cards d-flex justify-content-center mt-5">

            <div class="card rounded-5">

                <div class="card-image">
                    <img src="../../assets/smart1.png" alt="">
                </div>

                <div class="card-text">

                    <h3>3D modelling</h3>
                    <p>
                        We constantly ask questions. It helps us shape your story and deliver the results you creave. Yep, we'll drill deep to deliver above and beyond your expectations.
                    </p>

                </div>

            </div>

            <div class="card rounded-5 mx-4">

                <div class="card-image">
                    <img src="../../assets/smart2.png" alt="">
                </div>

                <div class="card-text">

                    <h3>3D modelling</h3>
                    <p>
                        We constantly ask questions. It helps us shape your story and deliver the results you creave. Yep, we'll drill deep to deliver above and beyond your expectations.
                    </p>

                </div>

            </div>

            <div class="card rounded-5">

                <div class="card-image">
                    <img src="../../assets/smart3.png" alt="">
                </div>

                <div class="card-text">

                    <h3>3D modelling</h3>
                    <p>
                        We constantly ask questions. It helps us shape your story and deliver the results you creave. Yep, we'll drill deep to deliver above and beyond your expectations.
                    </p>

               </div>

            </div>

        </div>

        <img class="image two" :src="getImg('smart4')" alt="">

    </div>
  </section>
</template>

<style lang="scss" scoped>
@use '../../scss/partials/var' as*;
.image{
        
        
}
.image.one{
    left: 0;
    width: 550px;
}
.image.two{
        position: absolute;
        right: 50px;
        width: 100px;
        transform: rotate(350deg);
}
.container_custom{
    position: absolute;
    right: 0 ;
    
    h1,
    h3{
        font-weight: 700;
    }
    .text{
        h3,
        h1{
            text-transform: capitalize ;
        }
        h1{
            font-size: 80px;
        }
        h3{
            color: $light-violet;
        }
    }
    .card{
        width: 250px;
        text-align: center;
        padding: 25px 10px 20px 10px;
        img{
            width: 60px;
        }
        .card-text{
            color: $violet;
        }
    }
    .card:first-child{
        background: linear-gradient(0deg, lighten($orange, 40%) 0%, $white 100%);
    }
    .card:nth-child(2){
        background: linear-gradient(0deg, lighten($violet, 75%) 0%, $white 100%);
    }
    .card:last-child{
        background: linear-gradient(0deg, lighten($pink, 2%) 0%, $white 100%);
    }
}

</style>