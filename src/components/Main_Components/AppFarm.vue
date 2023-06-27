<template>
    <div class="container">
        <div class="upper-text d-flex justify-content-between align-items-start">
            <div class="left-side">
                <h4 class="text-left">
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
    </div>
</template>
<script>
export default {
    
}
</script>
<style lang="scss" scoped>
@use '../../styles/partials/mixin' as *; 
@use '../../styles/partials/variables' as *;

.left-side{
    width: 50%;
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

</style>