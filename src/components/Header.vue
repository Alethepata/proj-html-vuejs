<script>
import TopBar from './partials/TopBar.vue';
import Jumbotron from './partials/Jumbotron.vue';
import Design from './partials/Design.vue';
import Video from './partials/Video.vue';
export default {
    name: 'Header',
    components: {
        TopBar,
        Jumbotron,
        Design,
        Video
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
        <Video/>
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