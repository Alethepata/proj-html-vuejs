<script>
import MenuList from './MenuList.vue';
import menu from '../../data/menu';
export default {
    name: 'TopBar',
    data() {
        return {
            menu
        }
    },
    components: {
        MenuList
    }
}
</script>

<template>
  <div class="container_custom">
    <div class="top-bar py-4 d-flex justify-content-between align-items-center  ">
        <div class="logo">
            <img src="/logo.png" alt="logo">
        </div>
        <div class="menu d-flex align-items-center">
            <nav>
                <ul class="d-flex align-items-center m-0 p-0">
                    <MenuList
                    v-for="(item,index) in menu"
                    :key="index"
                    :title="item.title"
                    :link="item.link"
                    />
                </ul>
            </nav>
            <button class="btn_custom_pink">Get a Quote</button>
        </div>

    </div>
  </div>
</template>

<style>

</style>