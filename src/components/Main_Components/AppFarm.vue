<template>
    <div class="container">
        <div class="upper-text d-flex justify-content-between align-items-start">
            <div class="left-side">
                <h4 class="text-left mb-4">
                    FARM TO TABLE
                </h4>
                <p class="text-left mb-5">
                    Aliquam erat volutpat. Ut quis ligula a magna blandit finibus. Suspendisse maximus lacus non nunc lacinia lobortis.
                </p>
            </div>
            <button class="title-jumbo">
                READ OUR BLOG
                <i class="ms-2 fa-solid fa-book-open"></i>
            </button>
        </div>
        <div class="image-wrapper d-flex">
            <div class="card-dish-big p-0">
                    <div class="img-container">
                        <img src="../../assets/img/single-post-img3-1200x790.jpg"/>
                    </div>
                    <div class="text-card-container">
                        <h4>
                            Food Corner: Top Japanese Restaurants for Sushi
                        </h4>
                        <p class="description mt-1">
                            By admin | March 25th, 2019
                        </p>
                        <div class="dotted-line my-4">
                        </div>
                        <p class="dish-recipe">
                            Suspendisse at semper odio. Nam fringilla scelerisque tincidunt. Orci varius natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Donec tincidunt posuere ornare. Phasellus placerat odio non feugiat sollicitudin. Integer vitae elementum ex. Sed porttitor, diam eget convallis volutpat, arcu tellus facilisis nulla, id dignissim orci leo id
                        </p>
                        <div class="lower-text-card d-flex justify-content-between py-4">
                            <span>
                                Read More
                                <i class="ms-2 fa-solid fa-chevron-right fa-xs"></i>
                            </span>
                            <i class="fa-regular fa-comments">
                                <span class="number-comment">0</span>
                            </i>
                        </div>          
                    </div>
            </div>
            <div class="card-group">
                <div class="latest-recipe">
                    <img class="mb-5" src="../../assets/img/ad-bg.jpg" alt="ad-bg">
                    <p class="recipe-text">
                        VIEW OUR LATEST RECIPES
                    </p>
                </div>
                <div class="card-container">
                        <img src="../../assets/img/singapore-featured-image-1200x790.jpg" alt="ad-bg">
                    <div class="text-center city-guide">
                        <i class="fa-solid fa-earth-americas me-2"></i>
                        <span>
                            VIEW ALL CITY GUIDES
                        </span>
                        <span class="title-singapore">
                            City Guide : Singapore
                        </span>
                    </div>
                </div>
                <div class="dotted-line my-4"></div>
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

.card-group{
    width: 30%;
    height: 100%;
    img{
        width: 100%;
    }
}
.left-side{
    width: 45%;
}
h4{
    font-weight: 200;
    font-size: 1rem;
}
p{
    font-weight: 200;
    color: $darkGrey;
}
button{
        background-color: $orange;
        padding: 0.8rem 2.5rem;
        color: $white;
        font-weight: 200;
        border-radius: 0.2rem;
        font-size: 0.9rem;
        border: none;
    }
    .card-dish-big{
    background-color: white;
    box-shadow: 0px 10px 15px -3px rgba(0,0,0,0.1);
    width: calc(70% - 4rem );
    height: 100%;
    margin-right: 4rem;
    h4{
        font-size: 1.3rem;
        margin-top: 1rem;
        font-family: 'Vidaloka', serif;
    }
    img{
        width: 100%;
        &:hover{
            opacity: 0.5;
            transition: 1s;
            background-color: radial-gradient(circle farthest-side, #fceabb, #f8b500);
        }
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
    .description{
        font-weight: 200;
    }
    .dish-recipe{
        color: $darkGrey;
        font-weight: 200;
    }
    .text-card-container{
    padding: 1rem 2.2rem;
}
}
.dotted-line{
        width: 100%;
        border: 1px dotted #e0dede;
    }

    .lower-text{

        span{

            font-weight: 200;
        }
    }
    .number-comment{
        font-size: 0.8rem;
        margin-left: 0.5rem;
    }
    .city-guide{
        background-color: $orange;
        color: white;
        padding: 1rem;
        font-size: 0.85rem;
        position: relative;
    }
    .title-singapore{
        font-weight: 200;
        background-color: rgba(0,0,0,0.8);
        padding: 0.65rem 2.3rem;
        font-size: 1.5rem;
        position: absolute;
        left: 0;
        bottom:100px
    }

    .latest-recipe{
        position: relative;
    }
        .recipe-text{
            text-align: center;
            position: absolute;
            left: 50%;
            bottom: 30%;
            transform: translate(-50% , - 50% );
            padding: 0 2rem;
            font-size: 1.7rem;
            color: black;
            font-weight: 200;
        }
</style>