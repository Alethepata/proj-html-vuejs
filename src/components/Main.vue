<script>
import FirstSection from './partials/FirstSection.vue';
export default {
    name: 'Main',
    components: {
        FirstSection
    }
}
</script>

<template>
  <main>
    <FirstSection/>
  </main>
</template>

<style lang="scss">
@use '../scss/partials/var' as*;
main{
    color: $violet;
}

</style>