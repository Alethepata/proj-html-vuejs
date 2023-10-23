<script>
import menuFooter from '../data/menuFooter';
import MenuList from './partials/MenuList.vue'
export default {
    name: 'Footer',
    data() {
        return {
            menuFooter
        }
    },
    components: {
        MenuList
    }
}
</script>

<template>
  <footer>
    <div class="container_custom">
        <div class="footer-top d-flex justify-content-between">
            <img src="footer-logo.png" alt="">
            <div class="menu">
                <nav>
                <ul class="d-flex align-items-center m-0 p-0">
                    <MenuList
                    v-for="(item,index) in menuFooter"
                    :key="index"
                    :title="item.title"
                    :link="item.link"
                    />
                </ul>
            </nav>
            </div>
        </div>
        <div class="footer-bottom d-flex justify-content-between">
            <p>
                Copyright 2002 <span>Softivus.</span> All rights reserved.
            </p>
            <div class="social">
                        <i class="fa-brands fa-facebook-f"></i>
                        <i class="fa-brands fa-twitter"></i>
                        <i class="fa-brands fa-instagram"></i>
                    </div>
        </div>
    </div>
  </footer>
</template>

<style lang="scss" scoped>
@use '../scss/partials/var' as*;

footer{
    margin-bottom: 20px;
    .footer-top{
        border-bottom: 1px solid lighten($grey, 30%);
        padding-bottom: 20px;
    }
    .footer-bottom{
        padding-top: 20px;
        p{
           span{
            color: $light-violet;
            font-weight: 700;
           } 
        }
    }
}
</style>