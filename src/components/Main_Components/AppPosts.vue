<template>
       <div class="container">
        <div class="image-wrapper d-flex flex-wrap">
            <div class="card-dish-social p-0 mb-5">
                    <div class="img-container">
                        <img src="../../assets/img/single-post-img3-1200x790.jpg"/>
                    </div>
                    <div class="text-card-container text-center">
                        <h4>
                            Food Corner: Top Japanese Restaurants for Sushi
                        </h4>
                        <p class="description mt-1">
                            By admin | March 25th, 2019
                        </p>  
                    </div>
            </div>
            <div class="card-dish-social p-0 mb-5">
                    <div class="img-container">
                        <img src="../../assets/img/single-post-img3-1200x790.jpg"/>
                    </div>
                    <div class="text-card-container text-center">
                        <h4>
                            Food Corner: Top Japanese Restaurants for Sushi
                        </h4>
                        <p class="description mt-1">
                            By admin | March 25th, 2019
                        </p>  
                    </div>
            </div>
            <div class="card-dish-social p-0 mb-5">
                    <div class="img-container">
                        <img src="../../assets/img/single-post-img3-1200x790.jpg"/>
                    </div>
                    <div class="text-card-container text-center">
                        <h4>
                            Food Corner: Top Japanese Restaurants for Sushi
                        </h4>
                        <p class="description mt-1">
                            By admin | March 25th, 2019
                        </p>  
                    </div>
            </div>
   <nav class="navbar bg-body-tertiary">
  <div class="container-fluid">
    <form class="d-flex" role="search">
      <input class="form-control me-2" type="search" placeholder="Search" aria-label="Search">
    </form>
  </div>
    </nav>
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
    .card-dish-social{
    background-color: white;
    box-shadow: 0px 10px 15px -3px rgba(0,0,0,0.1);
    width: calc(35% - 4rem );
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
    padding: 1rem 1.5rem;
}
}

</style>