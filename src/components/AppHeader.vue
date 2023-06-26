<template>
  <header>
    <div class="container header=wrapper">
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
    }
      },
}
</script>
<style lang="scss" scoped>
@use '../styles/partials/mixin' as *; 
@use '../styles/partials/variables' as *;

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
.container{
  max-width: 1200px;
}
header{
  background-color: $lightGrey;
  height: 250px;
  
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