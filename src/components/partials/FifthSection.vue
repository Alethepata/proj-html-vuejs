<script>
export default {
    name:'FifthSection',
    methods: {
        getImg(img) {
            return new URL (`../../assets/${img}.png`, import.meta.url).href
        }
    }
}
</script>

<template>
  <section>
    <div class="container_custom text-center">
        <div class="text">
            <h4>andidio magic team member</h4>
            <h1>let us animate your project</h1>
            <p>
                We create new worlds! Let's collaborate and create engaging, effective award-winning animations
            </p>
        </div>
        <div class="cards d-flex justify-content-between">
            <div class="card rounded-4">
                <div class="card-image">
                    <img :src="getImg('team1')" alt="">
                </div>
                <div class="card-text">
                    <h2>robert coleman</h2>
                    <p>owner & creative director</p>
                    <div class="social mt-5">
                        <i class="fa-brands fa-facebook-f"></i>
                        <i class="fa-brands fa-twitter"></i>
                        <i class="fa-brands fa-instagram"></i>
                    </div>
                </div>
            </div>
            <div class="card rounded-4">
                <div class="card-image">
                    <img :src="getImg('team2')" alt="">
                </div>
                <div class="card-text">
                    <h2>don woods</h2>
                    <p>administrator</p>
                    <div class="social mt-5">
                        <i class="fa-brands fa-facebook-f"></i>
                        <i class="fa-brands fa-twitter"></i>
                        <i class="fa-brands fa-instagram"></i>
                    </div>
                </div>
            </div>
            <div class="card rounded-4">
                <div class="card-image">
                    <img :src="getImg('team4')" alt="">
                </div>
                <div class="card-text">
                    <h2>tomas nash</h2>
                    <p>2d animator & compositor</p>
                    <div class="social mt-5">
                        <i class="fa-brands fa-facebook-f"></i>
                        <i class="fa-brands fa-twitter"></i>
                        <i class="fa-brands fa-instagram"></i>
                    </div>
                </div>
            </div>
        </div>
    </div>
    <div class="arrows d-flex justify-content-center my-5">
        <i class="fa-solid fa-arrow-left"></i>
        <div class="circles d-flex mx-4">
            <div class="circle"></div>
            <div class="circle mx-2"></div>
            <div class="circle"></div>
            <div class="circle ms-2 "></div>
        </div>
        <i class="fa-solid fa-arrow-right"></i>
    </div>

  </section>
</template>

<style lang="scss" scoped>
@use '../../scss/partials/var' as*;
.card{
    width: 30%;
    position: relative;
    margin-top: 150px;
    background-color: lighten($orange, 40%);
    border: 0;
    padding: 40px 0;
    h2,
    p{
        color: $violet;
    }
    p{
        text-transform: capitalize;
    }
    .card-image{
        position: absolute;
        left: 50%;
        transform: translate(-50%);
        top: -50px;
        
    }
    .card-text{
       margin-top: 150px; 
    }
}
.circle{
    background-color: $grey;
    width: 10px;
    height: 10px;
    border-radius: 50%;
    &:nth-child(2){
        background-color: $orange;
    }
}

</style>