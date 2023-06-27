<template>
    <div class="container">
        <div class="row">
            <div class="col-6 card-dish-big p-0">
                <div class="img-container">
                    <img src="../../assets/img/Yogurt-Nan.jpg"/>
                </div>
                <div class="text-card-container">
                    <h4>
                        Lunch Favourite with Salad, Naan And Beans
                    </h4>
                    <p class="description mt-1">
                        Bakery, Featured, Healthy, Latest Recipes, Staff Picks
                    </p>
                    <div class="dotted-line my-4">
                    </div>
                    <p class="dish-recipe">
                        Suspendisse at semper odio. Nam fringilla scelerisque tincidunt. Orci varius natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Donec tincidunt posuere ornare. Phasellus placerat odio non feugiat sollicitudin. Integer vitae elementum ex. Sed porttitor, diam eget convallis volutpat, arcu tellus facilisis nulla, id dignissim orci leo id
                    </p>            
                    <button>
                        LEARN MORE
                    </button>
                </div>
            </div>
            <div class="col-3 px-4 card-dish-big">
                <img :src="getImagePath(imageRecipe)" alt="">
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
<style lang="scss" scoped>
@use '../../styles/partials/mixin' as *; 
@use '../../styles/partials/variables' as *;


.img-container{
    width: 100%;
}
.text-card-container{
    padding: 1rem 2.2rem;
}

.card-dish-big{
    background-color: white;
    box-shadow: 0px 10px 15px -3px rgba(0,0,0,0.1);
    margin-right: 3rem;
    h4{
        font-size: 1.3rem;
        margin-top: 1rem;
        font-family: 'Vidaloka', serif;
    }
    img{
        width: 100%;
    }
    button{
        background-color: $orange;
        padding: 0.8rem 2.5rem;
        color: $white;
        font-weight: 200;
        border-radius: 0.15rem;
        font-size: 0.9rem;
        border: none;
        margin-bottom: 2rem;
    }
    .dotted-line{
        width: 100%;
        border: 1px dotted $dottedColor;
    }
    .description{
        font-weight: 200;
    }
    .dish-recipe{
        color: $darkGrey;
        font-weight: 200;
    }
}
</style>