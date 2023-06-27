<template>
     <h4 class="text-center mt-5">
            CULINARY COLLECTION
        </h4>
        <p class="text-center mb-5">
            Aliquam erat volutpat. Ut quis ligula a magna blandit finibus. Suspendisse maximus lacus non nunc lacinia lobortis.
        </p>
        <div class="container">
            <div class="row mx-auto justify-content-between">
                <AppCardCulinary v-for="card in listCard"
                :image="card.img"
                :text="card.text"
                />
            </div>
        </div>
</template>
<script>
import AppCardCulinary from './AppCardCulinary.vue';
export default {
    data() {
        return {
            listCard:[
                {
                    img:'https://avada.website/food/wp-content/uploads/sites/118/2019/08/drinks-recipes.png',
                    text:'DRINKS'
                },
                {
                    img:'https://avada.website/food/wp-content/uploads/sites/118/2019/08/soups-recipes.png',
                    text:'SOUPS'
                },
                {
                    img:'https://avada.website/food/wp-content/uploads/sites/118/2019/08/baking-recipes.png',
                    text:'BAKERY'
                },
                {
                    img:'https://avada.website/food/wp-content/uploads/sites/118/2019/08/dinner-recipes.png',
                    text:'DINNER'
                },
                {
                    img:'https://avada.website/food/wp-content/uploads/sites/118/2019/08/healthy-recipes.png',
                    text:'HEALTY'
                },
                {
                    img:'https://avada.website/food/wp-content/uploads/sites/118/2019/08/staff-picks.png',
                    text:'STAFF PICKS'
                },
                {
                    img:'https://avada.website/food/wp-content/uploads/sites/118/2019/08/premium-recipes.png',
                    text:'APPETISERS'
                },
                {
                    img:'https://avada.website/food/wp-content/uploads/sites/118/2019/08/quick-easy-recipes.png',
                    text:'QUICK & EASY'
                },
            ]
        }
    },
    components:{
        AppCardCulinary,
    }
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