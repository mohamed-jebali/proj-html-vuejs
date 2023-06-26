<template>
    <div class="container bg-white">
        <div class="foodie-wrapper">
            <h4 class="text-center">
                Foodie Journal
            </h4>
            <div class="box-foodie">
                <div class="single-box text-center">
                    <img src="../../assets/img/single-post-img3-600x395.jpg" alt="">
                    <p class="text-foodie">
                        Food Corner: Top Japanese Restaurants for Sushi
                    </p>
                    <p class="date-foodie">
                        By admin|March 25th, 2019
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

.foodie-wrapper{
    background-color: white;
    border: 1px solid black;
}
h4{
    padding: 1.5rem;
}
.box-foodie{
    display: flex;
    flex-wrap: wrap;
    background-color: white;
    border: 1px solid black;
    img{
        height: 265px;
    }
}
.single-box{
    width: calc(100% / 3);
}
.text-foodie{
    font-family: 'Vidaloka', serif;
    font-size: 1.3rem;
    padding: 0 4.5rem;
}
.date-foodie{
    font-family: 'Catamaran', sans-serif;
    font-size: 1rem;
    font-weight: 200;
}
</style>