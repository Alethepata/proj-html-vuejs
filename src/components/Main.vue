<script>
import FirstSection from './partials/FirstSection.vue';
import SecondSection from './partials/SecondSection.vue';
import ThirdSection from './partials/ThirdSection.vue';
import FourthSection from './partials/FourthSection.vue';
export default {
    name: 'Main',
    components: {
      FirstSection,
      SecondSection,
      ThirdSection,
      FourthSection
        
    }
}
</script>

<template>
  <main>
    <FirstSection/>
    <SecondSection/>
    <ThirdSection/>
    <FourthSection/>
  </main>
</template>

<style lang="scss">
@use '../scss/partials/var' as*;
main{
    color: $violet;
}

</style>