<template>
    <div class="container">
        <div class="row">
            <div class="col-6 card-dish-big">
                <img class="img-card" :src="getImagePath(imageRecipe)" alt="">
                <h4>
                    {{ titleRecipe }}
                </h4>
                <p class="description mt-3">
                    {{ descriptionRecipe }}
                </p>
                <div class="dotted-line my-4">
                </div>
                <p>
                    {{ dishRecipe }}
                </p>            
                <button>
                    {{buttonRecipe}}
                </button>
            </div>
            <div class="col-3 px-4 card-dish-big">
                <img :src="imageRecipe" alt="">
            </div>
            <div class="col-3 px-4 card-dish-big">
                <img :src="imageRecipe" alt="">
            </div>
        </div>
    </div>
</template>
<script>
export default {
    methods: {
        getImagePath: function(img) {
        return new URL(`../assets/img/${img}`, import.meta.url).href;
}
    },

    props:{
        imageRecipe:String,
        titleRecipe:String,
        descriptionRecipe:String,
        dishRecipe:String,
        buttonRecipe:String
    }
}
</script>
<style lang="scss">
@use '../../styles/partials/mixin' as *; 
@use '../../styles/partials/variables' as *;
.card-dish-big{
    background-color: white;
    box-shadow: 0px 10px 15px -3px rgba(0,0,0,0.1);
    h4{
        font-size: 1.3rem;
        font-family: 'Vidaloka', serif;
    }
    img{
        height: 50px;
    }
    button{
        background-color: $orange;
        padding: 0.5rem 2.5rem;
        color: $white;
        font-weight: 200;
        border-radius: 0.15rem;
        font-size: 0.9rem;
        border: none;
    }
    .dotted-line{
        width: 100%;
        border: 1px dotted $dottedColor;
    }
}
</style>