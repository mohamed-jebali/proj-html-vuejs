<template>
    <div>
        <h4 class="text-center">
            POPULAR RECIPES
        </h4>
        <p class="text-center">
            Aliquam erat volutpat. Ut quis ligula a magna blandit finibus. Suspendisse maximus lacus non nunc lacinia lobortis.
        </p>
        <AppRecipes v-for="recipe in listRecipes"
        :imageRecipe="recipe.img"
        :titleRecipe="recipe.title"
        :descriptionRecipe="recipe.description"
        :dishRecipe="recipe.dishText"
        :buttonRecipe="recipe.button"
        />
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
            listRecipes:[
                {
                    img:'../../assets/img/Yogurt-Nan.jpg',
                    title:'Lunch Favourite with Salad, Naan And Beans',
                    description:'Bakery, Featured, Healthy, Latest Recipes, Staff Picks',
                    dishText:'Suspendisse at semper odio. Nam fringilla scelerisque tincidunt. Orci varius natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Donec tincidunt posuere ornare. Phasellus placerat odio non feugiat sollicitudin. Integer vitae elementum ex. Sed porttitor, diam eget convallis volutpat, arcu tellus facilisis nulla, id dignissim orci leo id',
                    button:'LEARN MORE',

                },
            ]
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
    padding: 0 28rem;
    font-weight: 200;
    color: $darkGrey;
}
</style>