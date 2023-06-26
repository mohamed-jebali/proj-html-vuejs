<template>
    <div class="jumbo">
        <div class="box-jumbo mx-auto text-center">
            <span class="title-jumbo">
                TODAYS' PICK
            </span>
            <div class="text-jumbo">
                Food Corner: Top Japanese Restaurants for Sushi <br>
                March 25, 2019
            </div>
        </div>
    </div>
</template>
<script>
export default {
    
}
</script>
<style lang="scss">
@use '../styles/partials/mixin' as *; 
@use '../styles/partials/variables' as *;

    .jumbo{
        background-image: url(../assets/img/slide1-bg-66x66.jpg);
        background-size: cover;
        height: 300px;
        padding: 2rem 0;
    }
    .title-jumbo{
        background-color: $orange;
        padding: 0.5rem 2.5rem;
        color: $white;
        font-weight: 200;
        border-radius: 0.5rem;
        font-size: 0.9rem;
    }
    .text-jumbo{
        margin-top: 2rem;
        font-size: 2rem;
    }
    .box-jumbo{
        background-color: white;
        padding: 4rem;
        max-width: 600px;
        border-radius: 1rem;
    }
</style>