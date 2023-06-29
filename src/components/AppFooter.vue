<template>
  <div class="bg-wrapper">
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
          <ul class="list-info">
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
            <li>
              Contact
            </li>
          </ul>
        </div>
      </div>
      <div class="right-side d-flex">
        <div class="contact-us">
          <h4 class="orange">
            CONTACT US
          </h4>
          <ul class="contact-us-list">
            <li class="location">
              <i class="fa-solid fa-location-dot orange"></i>
              775 New York Ave, Brooklyn, Kings, New York 11203
            </li>
            <li>
              <i class="fa-solid fa-phone-flip orange"></i>
              + 0100-505-0000
            </li>
            <li>
              <i class="fa-solid fa-envelope orange"></i>
              info@your-domain.com
            </li>
          </ul>
        </div>
        <div class="get-our-app d-flex flex-column">
          <h4 class="orange">
            GET OUR APP
          </h4>
          <img src="../assets//img/download-app-store.png" alt="">
          <img src="../assets//img/download-android.png" alt="">
        </div>
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


.bg-wrapper{
  background-color: white;
  padding: 4rem 0;
}
.wrapper-brand-social{
  margin-right: 10rem;
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
      padding: 0;
      li{
        margin-bottom: 1rem;
      }
    }

    .orange{
    color: $orange;
}

.get-our-app{

  img{
    height: 60px;
    margin-bottom: 1rem;
  }
}
h4{
    font-size: 1rem;
    font-weight: 200;
  }

  .contact-us{
    margin-right: 2rem;
  }

  .list-info{
    li{
      font-weight: 200;
      &:hover{
        color: $orange;
        transition: 1s;
      }
    }
  }

  .contact-us-list{

    .location{
      text-indent: -1rem;
    }
    li{
      border-bottom: 0.5px solid #dfdfdd;
      padding-bottom: 1.2rem;
      width: 75%;
      font-weight: 200;
      color:$darkGrey;

      i{
        margin-right: 1rem;
      }
    }
  }
  </style>