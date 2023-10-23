<script>
export default {
  name: 'SixthSection',   
  methods: {
        getImg(img) {
            return new URL (`../../assets/${img}.png`, import.meta.url).href
        }
    }
}
</script>

<template>
  <section>
    <div class="container_custom">
      <div class="col text-center">
        <h4>why andidio studio</h4>
        <h1>we love our clients</h1>
        <p>
          We are trusted thrpughout adland an have a wealth of recommendations from start-ups to renowed global brands.
        </p>
      </div>
      <div class="cards d-flex justify-content-evenly mt-5">
        <div class="card">
          <img :src="getImg('sponsor5')" alt="">
        </div>
        <div class="card">
          <img :src="getImg('sponsor6')" alt="">
        </div>
        <div class="card">
          <img :src="getImg('sponsor1')" alt="">
        </div>
        <div class="card">
          <img :src="getImg('sponsor2')" alt="">
        </div>
        <div class="card">
          <img :src="getImg('sponsor3')" alt="">
        </div>
      </div>
    </div>
  </section>
</template>

<style lang="scss" scoped>
.card{
  border: none;
}
</style>