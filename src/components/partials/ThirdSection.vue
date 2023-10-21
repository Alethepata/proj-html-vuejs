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
    
  </section>
</template>

<style lang="scss" scoped>
@use '../../scss/partials/var' as*;


</style>