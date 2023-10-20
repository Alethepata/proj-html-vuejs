<script>
export default {
    name:'Jumbotron'
}
</script>

<template>
  <div class="container_custom text-center">
    <div class="text">
        <h5>imagine, create, experience</h5>
        <h1>we animate with ninja-like precision </h1>
        <p>
                We are character-driven animation studio striving to make high-quality animations.

        </p>
    </div>
    <div class="btn my-4">
        <button class="btn_custom_pink me-4">Start a Project</button>
        <button class="btn_custom">Portfolio</button>
    </div>
  </div>
</template>

<style lang="scss" scoped>
@use '../../scss/partials/var' as *;

.container_custom{
    padding-top:100px;
}
.text{
    color: $white;

    h5,
    h1{
        text-transform: capitalize; 
        font-weight: 700; 
    }
    

    h5{
    color: $orange;
    }  
    h1{
        
        font-size: 90px;
    }  
    p{
        font-weight: 400;
        font-size: 25px;
    }
    
}

</style>