<script>
import TopBar from './partials/TopBar.vue';
import Jumbotron from './partials/Jumbotron.vue';
import Design from './partials/Design.vue';
export default {
    name: 'Header',
    components: {
        TopBar,
        Jumbotron,
        Design
    }
}
</script>

<template>
    <header>
        
        <div class="header_top position-relative">
            <Design/>
            <div class="content position-absolute">
                <TopBar/>
                <Jumbotron/>
            </div>
        </div>
    </header>
</template>

<style lang="scss">
.header_top{
    background-image: url(../assets/preloader.png);
    background-size: cover;
    .content{
        top: 0;
        left: 50%;
        transform: translate(-50%);
        width: 100%;
    }
}

</style>