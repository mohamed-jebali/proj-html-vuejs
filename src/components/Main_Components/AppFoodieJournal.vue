<template>
    <div class="container bg-white">
        <div class="foodie-wrapper">
            <h4 class="text-center">
                FOODIE JOURNAL
            </h4>
            <div class="box-foodie">
                <div class="single-box text-center">
                    <img src="../../assets/img/single-post-img3-600x395.jpg" alt="single-post-3">
                    <p class="text-foodie">
                        Food Corner: Top Japanese Restaurants for Sushi
                    </p>
                    <p class="date-foodie">
                        By admin | March 25th, 2019
                    </p>
                </div>
                <div class="single-box text-center">
                    <img src="../../assets/img/fi-roundup-600x395.jpg" alt="roundup-image">
                    <p class="text-foodie">
                        Roundup: My New Favourite Recipes For Healthy Living
                    </p>
                    <p class="date-foodie">
                        By admin | March 25th, 2019
                    </p>
                </div>
                <div class="single-box text-center">
                    <img src="../../assets/img/fi-toasts-600x395.jpg" alt="fi-toasts-image">
                    <p class="text-foodie">
                        Why These Toasts with Tea are My New Favorite
                    </p>
                    <p class="date-foodie">
                        By admin | March 25th, 2019
                    </p>
                </div>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    name:"AppFoodieJournal",
    
}
</script>
<style lang="scss" scoped>

.container{
    position: relative;
    bottom: 4rem;
    box-shadow: 0px 10px 15px -3px rgba(0,0,0,0.1);
}
.foodie-wrapper{
    background-color: white;
}
h4{
    padding: 1.1rem;
    font-size: 1.1rem;
    font-weight: 200;
}
.box-foodie{
    display: flex;
    flex-wrap: wrap;
    img{
        height: 225px;
    }
}
.single-box{
    width: calc(100% / 3);
}
.text-foodie{
    font-family: 'Vidaloka', serif;
    font-size: 1.3rem;
    margin-top: 1rem;
    padding: 0 4.5rem;
}
.date-foodie{
    font-family: 'Catamaran', sans-serif;
    font-size: 1rem;
    font-weight: 200;
}
</style>