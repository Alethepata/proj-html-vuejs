<script>
import FirstSection from './partials/FirstSection.vue';
import SecondSection from './partials/SecondSection.vue';
import ThirdSection from './partials/ThirdSection.vue';
export default {
    name: 'Main',
    components: {
      FirstSection,
      SecondSection,
      ThirdSection
        
    }
}
</script>

<template>
  <main>
    <FirstSection/>
    <SecondSection/>
    <ThirdSection/>
  </main>
</template>

<style lang="scss">
@use '../scss/partials/var' as*;
main{
    color: $violet;
}

</style>