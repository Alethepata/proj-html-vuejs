<script>
import TopBar from './partials/TopBar.vue';
import Jumbotron from './partials/Jumbotron.vue';
export default {
    name: 'Header',
    components: {
        TopBar,
        Jumbotron
    }
}
</script>

<template>
    <header>
        <TopBar/>
        <Jumbotron/>
    </header>
</template>

<style lang="scss">
header{
    font-size: 20px;
    font-weight: bold;
}

</style>