<script>
import FirstSection from './partials/FirstSection.vue';
import SecondSection from './partials/SecondSection.vue';
import ThirdSection from './partials/ThirdSection.vue';
import FourthSection from './partials/FourthSection.vue';
import FifthSection from './partials/FifthSection.vue';
import SixthSection from './partials/SixthSection.vue';
import SeventhSection from './partials/SeventhSection.vue';
export default {
    name: 'Main',
    components: {
      FirstSection,
      SecondSection,
      ThirdSection,
      FourthSection,
      FifthSection,
      SixthSection,
      SeventhSection
        
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