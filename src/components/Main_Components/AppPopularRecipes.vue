<template>
    <div>
        <h4 class="text-center">
            POPULAR RECIPES
        </h4>
        <p class="text-center mb-5">
            Aliquam erat volutpat. Ut quis ligula a magna blandit finibus. Suspendisse maximus lacus non nunc lacinia lobortis.
        </p>
        <AppRecipes/>
    </div>
</template>
<script>
 import AppRecipes from './AppRecipes.vue';
export default {
    name:'AppPopularRecipes',
    components:{
        AppRecipes,
    },
    data() {
        return {
        }
    },
}
</script>
<style lang="scss" scoped>
@use '../../styles/partials/mixin' as *; 
@use '../../styles/partials/variables' as *;

h4{
    font-weight: 200;
    font-size: 1rem;
    margin-bottom: 1.5rem;
}
p{
    padding: 0 25rem;
    font-weight: 200;
    color: $darkGrey;
}
</style>