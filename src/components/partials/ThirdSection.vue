<script>
export default {
    name: 'ThirdSection',
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
        <div class="row">
            <div class="col">
                <h4>our works</h4>
                <h1>featured productions</h1>
                <p>
                    Here's just a small sample of some of those projects that we're proud of.
                    If you're looking for something specific feel to get in conctact with us
                </p>
            </div>
        </div>
        <div class="row row-cols-2">
            <div class="col mb-4">
                <img :src="getImg('work1')" alt="">
            </div>
            <div class="col">
                <img :src="getImg('work2')" alt="">
            </div>
            <div class="col">
                <img :src="getImg('work3')" alt="">
            </div>
            <div class="col">
                <img :src="getImg('work4')" alt="">
            </div>
        </div>
        <div class="row mt-5">
            <div class="col">
                <button class="btn_custom_grey text-capitalize">see our work</button>
            </div>
        </div>
    </div>
  </section>
</template>

<style lang="scss" scoped>
@use '../../scss/partials/var' as*;
img{
    width: 100%;
}
</style>