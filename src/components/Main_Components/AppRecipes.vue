<template>
    <div class="container">
        <div class="row">
            <div class="card-dish-big p-0">
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
            <div class="container-single-dish d-flex">
                <div class="single-dish">
                    <img src="../../assets/img/Mixed-fruits-1200x790.jpg" alt="rachel-park-dish">
                </div>
                <div class="single-dish">
                    <img src="../../assets/img/r-rachel-park-366508-unsplash-min-1200x790.jpg" alt="rachel-park-dish">
                </div>
                <div class="single-dish">
                    <img src="../../assets/img/r-michelle-tsang-500721-unsplash-min-600x395.jpg" alt="rachel-park-dish">
                </div>
                <div class="single-dish">
                    <img src="../../assets/img/quick-summer-drink-460x295.jpg" alt="rachel-park-dish">
                </div>
                <div class="single-dish">
                    <img src="../../assets/img/r-maarten-van-den-heuvel-400626-unsplash-min-460x295.jpg" alt="rachel-park-dish">
                </div>
                <div class="single-dish">
                    <img src="../../assets/img/perfect-cosmopolitan-460x295.jpg" alt="rachel-park-dish">
                </div>
                <div class="single-dish">
                    <img src="../../assets/img/fi2x-6-460x295.jpg" alt="rachel-park-dish">
                </div>
                <div class="single-dish">
                    <img src="../../assets/img/r-brooke-lark-96398-unsplash-min-460x295.jpg" alt="rachel-park-dish">
                </div>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    methods: {
        
    },
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

.container-single-dish{
    width: calc(100% / 2);
    display: flex;
    justify-content: space-between;
    flex-wrap: wrap;
    height: 100%;
}
.single-dish{
    width: calc(100% / 2);
    border-left: 1.5rem solid #f5f5f1;
    height: 100%;
    margin-bottom: 1.7rem;
    img{
        width: 100%;
        &:hover{
            opacity: 0.5;
            transition: 1s;
            background-color: radial-gradient(circle farthest-side, #fceabb, #f8b500);
        }
    }
}
.card-dish-big{
    background-color: white;
    box-shadow: 0px 10px 15px -3px rgba(0,0,0,0.1);
    width: calc(100% / 2 - 1rem);
    height: 100%;
    margin-right: 1rem;
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
        margin-bottom: 1rem;
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