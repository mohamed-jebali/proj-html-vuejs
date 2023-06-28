<template>
        <div class="card-dish-social p-0 mb-5">
                    <div class="img-container">
                        <img :src="image"/>
                    </div>
                    <div class="text-card-container text-center">
                        <h4>
                            {{ title }}
                        </h4>
                        <p class="description mt-1">
                            {{ date }}
                        </p>  
                    </div>
        </div>
</template>
<script>
export default {
    props:{
        image:String,
        title:String,
        date:String
    }
}
</script>
<style lang="scss" scoped>
@use '../../styles/partials/mixin' as *; 
@use '../../styles/partials/variables' as *;

h4{
    font-weight: 200;
    font-size: 1rem;
}
p{
    font-weight: 200;
    color: $darkGrey;
}
    .card-dish-social{
    background-color: white;
    box-shadow: 0px 10px 15px -3px rgba(0,0,0,0.1);
    width: calc(35% - 3rem );
    height: 400px;
    margin-right: 3rem;
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
    .text-card-container{
    padding: 1rem 2.8rem;
}
}

</style>