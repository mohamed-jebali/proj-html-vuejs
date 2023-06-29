<template>
  <header>
    <div class="container header-wrapper d-none d-md-block ">
      <div class="row">
        <div class="col-12">
          <div class="upper-header d-flex justify-content-between pt-4">
            <div class="left-side d-flex">
              <span>
                Download App <span class="ios me-4">iOS</span>
              </span>
              <span>
                Advertise with us
              </span>
            </div>
            <div class="brand">
              <img src="../assets/img/avada-food-logo.png" alt="brand-logo-food-avada">
            </div>
            <div class="right-side d-flex">
              <img class="socials-icon" src="../assets/socials/facebook.svg" alt="facebook-logo" title="facebook">
              <img class="socials-icon" src="../assets/socials/instagram.svg" alt="instagram-logo" title="Instagram">
              <img class="socials-icon" src="../assets/socials/twitter.svg" alt="twitter-logo" title="Twitter">
              <img class="socials-icon" src="../assets/socials/youtube.svg" alt="youtube-logo" title="YouTube">
              <img class="socials-icon" src="../assets/socials/tiktok.svg" alt="tiktok-logo" title="TikTok">
              <img class="socials-icon" src="../assets/socials/pinterest.svg" alt="pinterest-logo" title="Pinterest">
            </div>
          </div>
        </div>
      </div>
      <nav>
      <ul class='d-flex justify-content-between'>
                    <li v-for="liElements,index in headerList" :class="liElements.active === true ? 'activeColor' : ''" @click='toggleActive(index)'>
                        {{liElements.text}}
                    </li>
                    <li>
                      <i class="fa-solid fa-magnifying-glass"></i>
                    </li>
      </ul>
    </nav>
    </div>
    <div class="mobile d-md-none">
      <div class="container">
        <div class="row justify-content-between align-items-center">
          <div class="col-12 d-flex justify-content-between">
            <img class="brand-mobile" src="../assets/img/avada-food-logo-mob-2x.png" alt="avada-mobile">
  <div class="dropdown">
  <i @click="clickAnimation()" class="fa-solid fa-burger fa-2x" type="button" data-bs-toggle="dropdown" aria-expanded="false"></i>
  <i @click="clickAnimation()" class="fa-solid fa-solid fa-xmark fa-2x d-none" type="button" data-bs-toggle="dropdown" aria-expanded="false"></i>
  <div class="dropdown-menu">
    <div><button class="dropdown-item bg-orange" type="button">Home</button></div>
    <div><button class="dropdown-item" type="button">Recipes</button></div>
    <div><button class="dropdown-item" type="button">Places</button></div>
    <div><button class="dropdown-item" type="button">Blog</button></div>
    <div><button class="dropdown-item" type="button">About</button></div>
    <div><button class="dropdown-item" type="button">Contact</button></div>
    <nav class="navbar">
                  <form class="d-flex align-items-center" role="search">
                    <i class="fa-solid fa-magnifying-glass mx-3"></i>
                    <input class="form-control me-2" type="search" placeholder="Search..." aria-label="Search">
                  </form>
                </nav>
  </div>
 </div>
          </div>
        </div>
      </div>
    </div>
  </header>
</template>
<script>
export default {
  data(){
        return{
            headerList:[
                {
                    text:"Home",
                    active: true
                },
                {
                    text:"Recipes",
                    active: false,
                },
                {
                    text:"Places",
                    active: false,
                },
                {
                    text:"Blog",
                    active: false,
                },
                {
                    text:"About",
                    active: false,
                },
                {
                    text:"Contact",
                    active: false,
                },
            ],

        }
      },
      methods: {
        toggleActive(index) {
        this.headerList.forEach((item, i) => {
        item.active = i === index;
      });
    },
    clickAnimation(){
        document.querySelector('.fa-burger').classList.toggle('clickAnimation')
      },
      },
}
</script>
<style lang="scss" scoped>
@use '../styles/partials/mixin' as *; 
@use '../styles/partials/variables' as *;

.navbar{
    .form-control{
        padding: 0.8rem;
        width: 330px;
        border: none;
        
    }
}
form{
  margin: auto;
    border: 2px solid  #dfdfdd;
    border-radius: 0.5rem;
    background-color: white;
    color: #dfdfdd;
    i{
        font-size: 1.1rem;
    }

    ::placeholder{
        color: #dfdfdd;       
    }
}

nav{
  padding-top: 3rem;
  max-width: 600px;
  margin: auto;
  font-weight: 200;
  ul li{
    &:hover{
            color: $orange;
            transition: 0.5s;
        }
  }
}
.brand-mobile{
  height: 60px;
  margin: 0.5rem 0.5rem;
}
.dropdown-menu{
  border: none;
  border-radius: 0;
  width: 450px;
  margin-top: 1.3rem !important;
}

.bg-orange{
    background-color: $orange;
    color: white;
  }
.dropdown-item{
  font-size: 0.85rem;
  font-weight: 200;
  text-align: center;
  margin-bottom: 0.1rem;
  padding: 0.8rem 0;
  &:hover{
    background-color: $orange;
    color: white;
    transition: 0.5s;
  }
}

.fa-burger{
  margin: 1.5rem 0.5rem;
}
.fa-xmark{
  margin: 1.5rem 0.5rem;
}
.clickAnimation{
    rotate: 2turn;
    transition: 0.5s;
    opacity: (0);
  }
header{
  background-color: $lightGrey;
  
  .left-side{
    font-size: 0.85rem;
    font-weight: 300;
    span{
      &:hover{
            color: $orange;
            transition: 0.5s;
        }
    }
    .ios{
      background-color: $orange;
      padding: 0.05rem 0.35rem;
      border-radius: .25rem;
      color: $white;
      font-size: 0.6rem;
      margin-left: 0.25rem;
    }
  }
  .right-side{

    .socials-icon{
      height: 35px;
      margin-right: 0.25rem;
      &:hover{
        background-color: white;
        border-radius: 0.25rem;
        transition: 1s;
      }
    }
  }
}
</style>