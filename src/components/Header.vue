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

<style>

</style>