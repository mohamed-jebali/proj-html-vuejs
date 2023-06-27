<template>
    <div class="jumbo">
        <div class="box-jumbo mx-auto text-center">
            <button class="title-jumbo">
                TODAYS' PICK
            </button>
            <div class="text-jumbo">
                Food Corner: Top Japanese Restaurants for Sushi
                <p class="date-jumbo">
                    March 25, 2019
                </p>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    
}
</script>
<style lang="scss" scoped>
@use '../../styles/partials/mixin' as *; 
@use '../../styles/partials/variables' as *;

    .jumbo{
        background-image: url(https://avada.website/food/wp-content/uploads/sites/118/2019/02/slide1-bg.jpg);
        background-size: cover;
        background-position: top;
        height: 500px;
        padding: 10rem 0;
        background-attachment: fixed;
    }
    .title-jumbo{
        background-color: $orange;
        padding: 0.5rem 2.5rem;
        color: $white;
        font-weight: 200;
        border-radius: 0.5rem;
        font-size: 0.9rem;
        position: relative;
        bottom: 15px;
        border: none;
    }
    .text-jumbo{
        margin-top: 0.5rem;
        font-size: 2.5rem;
        font-family: 'Vidaloka', serif;
        padding: 0 2rem;
        &:hover{
            color: $orange;
            transition: 0.5s;
        }
    }
    
    .box-jumbo{
        background-color: white;
        max-width: 680px;
        border-radius: 1rem;
    }
    .date-jumbo{
        font-family: 'Catamaran', sans-serif;
        font-size: 1rem;
        font-weight: 200;
        padding-bottom: 2rem;
        padding-top: 0.5rem;
        color: $darkGrey;
        &:hover{
            color: $darkGrey;
            transition: 0.5s;
        }
    }
</style>