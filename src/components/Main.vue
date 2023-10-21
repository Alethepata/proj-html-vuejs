<script>
import FirstSection from './partials/FirstSection.vue';
import SecondSection from './partials/SecondSection.vue';
export default {
    name: 'Main',
    components: {
      FirstSection,
      SecondSection
        
    }
}
</script>

<template>
  <main>
    <FirstSection/>
    <SecondSection/>
  </main>
</template>

<style lang="scss">
@use '../scss/partials/var' as*;
main{
    color: $violet;
}

</style>