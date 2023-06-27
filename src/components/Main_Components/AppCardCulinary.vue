<template>
            <div class="card mx-auto text-center mb-5">
                <img class="mx-auto" :src="image" alt="text">
                <p class="text-card">
                    {{ text }}
                </p>
            </div>
</template>
<script>
export default {
    props:{
        image:String,
        text:String
    }
}
</script>
<style lang="scss" scoped>
@use '../../styles/partials/mixin' as *; 
@use '../../styles/partials/variables' as *;
.card{
    background-color: white;
    width: calc(100% / 4 - 3rem);
    padding: 0.8rem 0;
    margin-right: 3rem;
    margin-bottom: 2rem;
    border-radius: 0;
    font-weight: 200;
    border: none;
    box-shadow: 0px 10px 15px -3px rgba(0,0,0,0.1);

    .text-card{
        width: 95%;
        margin: auto;
        padding: 0.2rem;
        &:hover{
            background-color: $orange;
            color: white;
            transition: 0.5s;
        } 
    }

    img{
        width: 35%;
        margin-bottom: 1rem;
        &:hover{
            scale: (1.1);
            transition: 1s;
        }
    }
}
</style>