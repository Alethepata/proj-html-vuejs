<script>
export default {
    name: 'MenuList',
    props: {
        title: String,
        link: String
    }
}
</script>

<template>
    <li class="me-4">
        <a :href="link">
            {{ title }}
        </a>
    </li>
</template>

<style lang="scss">
@use '../../scss/partials/var' as*;

a:hover{
    color: $orange;
}


</style>