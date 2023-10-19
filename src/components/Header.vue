<script>
import TopBar from './partials/TopBar.vue';
export default {
    name: 'Header',
    components: {
        TopBar
    }
}
</script>

<template>
    <header>
        <TopBar/>
    </header>
</template>

<style lang="scss">
header{
    font-size: 20px;
    font-weight: bold;
}

</style>