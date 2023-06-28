<template>
    <div class="wrapper-cards d-flex">
        <div class="card-dish">
            <img src="https://avada.website/food/wp-content/uploads/sites/118/2019/03/Yogurt-Nan.jpg" alt="yogurt-nan-image">  
        </div>
        <div class="card-dish">
            <img src="https://avada.website/food/wp-content/uploads/sites/118/2019/03/Mixed-fruits.jpg" alt="mixed-fruits-image">  
        </div>
        <div class="card-dish">
            <img src="https://avada.website/food/wp-content/uploads/sites/118/2019/03/r-rachel-park-366508-unsplash-min.jpg" alt="rachel-park-image">  
        </div>
        <div class="card-dish">
            <img src="https://avada.website/food/wp-content/uploads/sites/118/2019/03/r-michelle-tsang-500721-unsplash-min.jpg" alt="michelle-tsang-image">  
        </div>
    </div>
</template>
<script>
export default {
    
}
</script>
<style lang="scss">


.wrapper-cards{
    margin-bottom: 5rem;
}
.card-dish{
    width: calc(100% / 4);
    height: 100%;


    img{
        width: 100%;
    }
}

</style>