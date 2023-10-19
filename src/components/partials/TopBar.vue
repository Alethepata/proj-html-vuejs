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
    <div class="row">
        <div class="col-3">
            <img src="/logo.png" alt="logo">
        </div>
        <div class="col">
            <nav>
                <ul class="d-flex justify-content-between">
                    <MenuList
                    v-for="(item,index) in menu"
                    :key="index"
                    :title="item.title"
                    :link="item.link"
                    />
                </ul>
            </nav>
        </div>
        <div class="col-2">
            <button class="btn_custom_pink">Get a Quote</button>
        </div>
    </div>
  </div>
</template>

<style lang="scss">
@use '../../scss/partials/var' as*;
.btn_custom_pink{
    background-color: $pink;
    &:hover{
        background: none;
        border: 1px solid $white;
        color: $white;
    }
}
</style>