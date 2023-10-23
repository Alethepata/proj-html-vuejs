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
    <li class="ms-4">
        <a :href="link">
            {{ title }}
        </a>
    </li>
</template>

<style lang="scss" scoped>
@use '../../scss/partials/var' as*;
a{
    font-size: 20px;
    font-weight: bold;
}
a:hover{
    color: $orange;
}


</style>