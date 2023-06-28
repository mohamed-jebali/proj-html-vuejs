<template>
    <div class="container d-flex justify-content-between">
      <div class="left-side d-flex">
        <div class="wrapper-brand-social">
          <img class="brand" src="https://avada.website/food/wp-content/uploads/sites/118/2019/08/avada-food-logo-mob-2x.png" alt="food-avana-logo">
          <div class="socials">
            <img class="socials-icon" src="../assets/socials/facebook.svg" alt="facebook-logo" title="facebook">
            <img class="socials-icon" src="../assets/socials/instagram.svg" alt="instagram-logo" title="Instagram">
            <img class="socials-icon" src="../assets/socials/twitter.svg" alt="twitter-logo" title="Twitter">
            <img class="socials-icon" src="../assets/socials/youtube.svg" alt="youtube-logo" title="YouTube">
          </div>
        </div>
        <div class="list">
          <ul>
            <li>
              Recipes
            </li>
            <li>
              Places
            </li>
            <li>
              Blogs
            </li>
            <li>
              About
            </li>
            <li class="orange">
              Contact
            </li>
          </ul>
        </div>
      </div>
    </div>
  </template>
  <script>
  export default {
    
  }
  </script>
  <style lang="scss" scoped>

@use '../styles/partials/mixin' as *; 
@use '../styles/partials/variables' as *;

.wrapper-brand-social{
  margin-right: 4rem;
}
.socials-icon{
      height: 35px;
      margin-right: 0.25rem;
      &:hover{
        background-color: white;
        border-radius: 0.25rem;
        transition: 1s;
      }
    }

    .brand{
      height: 80px;
      margin-bottom: 2rem;
    }

    ul{
      li{
        margin-bottom: 1rem;
      }
    }

    .orange{
    color: $orange;
}
  </style>