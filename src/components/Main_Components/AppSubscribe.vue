<template>
    <div class="subscribe-container d-flex">
        <div class="text-wrapper mx-auto">
            <h3>
                Subscribe <span class="orange"> &</span> Receive A Free eBook
            </h3>
            <p class="text-sub">
                Aliquam erat volutpat. Ut quis ligula a magna blandit finibus. Suspendisse maximus lacus non nunc lacinia lobortis.
            </p>
<nav class="navbar">
<div class="mx-auto">
    <form class="d-flex align-items-center" role="search">
      <input class="form-control me-2" type="search" placeholder="Insert your email here...*" aria-label="Search">
      <button  type="submit">SUBSCRIBE</button>
    </form>
</div>
</nav>
<p class="last-sub-info mx-auto text-center mt-5">
    Cras porttitor pellentesque sem eu pretium.
</p>
        </div>
    </div>
</template>
<script>
export default {
    
}
</script>
<style lang="scss">

@use '../../styles/partials/mixin' as *; 
@use '../../styles/partials/variables' as *;

.subscribe-container{
    background-image: url(../../assets/img/subscribe-sec-bg.png);
    background-size: cover;
    height: 400px;
}



h3{
    font-family: 'VidaLoka';
    font-size: 1.5rem;
    text-align: center;
}

.orange{
    color: $orange;
}

.text-wrapper{
    max-width: 900px;
    margin: auto;
}
.text-sub{
    margin-top: 2rem;
    padding: 0 10rem;
    text-align: center;
    color: $darkGrey;
    font-weight: 200;
}

.navbar{

    .form-control{
        padding: 0.85rem;
        width: 400px;
        border: 2px solid  #dfdfdd;
        color: $darkGrey;

        ::placeholder{
          color: #dfdfdd;       
       }
    }
}

.last-sub-info{
    color: $darkGrey;
    font-weight: 200;
}

button{
        background-color: $orange;
        padding: 0.85rem 2.5rem;
        color: $white;
        font-weight: 200;
        font-size: 0.9rem;
        border: none;
    }

    
</style>