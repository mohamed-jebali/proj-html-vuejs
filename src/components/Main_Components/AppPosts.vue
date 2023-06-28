<template>
       <div class="container mx-auto">
        <div class="wrapper-posts d-flex">
            <div class="image-wrapper">
                <AppSinglePost class="d-flex flex-wrap" v-for="post in listPosts"
                :image="post.image"
                :title="post.title"
                :date="post.date"
                />
        <button class="load-posts">
            LOAD MORE POSTS
        </button>
            </div>
            <div class="right-wrapper-posts">
                <nav class="navbar">
                  <form class="d-flex align-items-center" role="search">
                    <i class="fa-solid fa-magnifying-glass mx-3"></i>
                    <input class="form-control me-2" type="search" placeholder="Search..." aria-label="Search">
                  </form>
                </nav>
                <div class="socials-box">
                    <p>
                        Follow Us
                    </p>
           <div class="social-container d-flex mb-3">
           <img class="socials-icon" src="../../assets/socials/facebook.svg" alt="facebook-logo" title="facebook">
          <img class="socials-icon" src="../../assets/socials/instagram.svg" alt="instagram-logo" title="Instagram">
          <img class="socials-icon" src="../../assets/socials/twitter.svg" alt="twitter-logo" title="Twitter">
          <img class="socials-icon" src="../../assets/socials/youtube.svg" alt="youtube-logo" title="YouTube">
          <img class="socials-icon" src="../../assets/socials/pinterest.svg" alt="pinterest-logo" title="Pinterest">
          </div>
          <div class="chat-box">
            <div class="upper-box-chat d-flex">
                <span class="me-5">
                    Popular
                </span>
                <div class="divider">

                </div>
                <span class="ms-5">
                    Recent
                </span>
            </div>
            <div class="contacts-comment">
                <div class="comment d-flex">
                    <img class="rounded-circle me-4 img-fluid mt-5" src="https://avada.website/food/wp-content/uploads/sites/118/2019/03/single-post-img3-150x150.jpg" alt="single-post-img-3">
                    <div class="text-box">
                        <p class="detail-comment">
                            Food Corner: Top Japanese Restaurants for Sushi <br>
                            <span class="date">
                                March 25th, 2019
                            </span>
                        </p>
                    </div>
                </div>
                <div class="comment d-flex">
                    <img class="rounded-circle me-4 img-fluid mt-5" src="https://avada.website/food/wp-content/uploads/sites/118/2019/02/singapore-featured-image-150x150.jpg" alt="singapore-image">
                    <div class="text-box">
                        <p class="detail-comment">
                            City Guide: Singapore <br>
                            <span class="date">
                                February 27th, 2019 
                            </span>
                        </p>
                    </div>
                </div>
                <div class="comment d-flex">
                    <img class="rounded-circle me-4 img-fluid mt-5" src="https://avada.website/food/wp-content/uploads/sites/118/2019/03/fi-toasts-150x150.jpg" alt="fi-toast-image">
                    <div class="text-box">
                        <p class="detail-comment">
                            Why These Toasts with Tea are My New Favorite <br>
                            <span class="date">
                                March 25th, 2019
                            </span>
                        </p>
                    </div>
                </div>
            </div>
            <div class="twitter-box">
                twitter box
            </div>
          </div>
                </div>
            </div>
        </div>
        </div>
</template>
<script>
import AppSinglePost from './AppSinglePost.vue';
export default {
    components:{
    AppSinglePost
},
    data() {
        return {
            listPosts:[
                {
                    image:'https://avada.website/food/wp-content/uploads/sites/118/2019/03/fi-roundup.jpg',
                    title:'Roundup: My New Favourite Recipes For Healthy Living',
                    date:'By admin | March 25th, 2019'
                },
                {
                    image:'https://avada.website/food/wp-content/uploads/sites/118/2019/03/fi-korean-food.jpg',
                    title:'Meal Prep: Korean Bibimbap with Kimchi',
                    date:'By admin | March 25th, 2019'
                },
                {
                    image:'https://avada.website/food/wp-content/uploads/sites/118/2019/03/fi-toasts.jpg',
                    title:'Why These Toasts with Tea are My New Favorite',
                    date:'By admin | March 25th, 2019'
                },
                {
                    image:'https://avada.website/food/wp-content/uploads/sites/118/2019/03/fi-street-food.jpg',
                    title:'Exploring Street Food in Bangkok',
                    date:'By admin | March 25th, 2019'
                },
                {
                    image:'https://avada.website/food/wp-content/uploads/sites/118/2019/03/fi-organic-breakfast.jpg',
                    title:'Organic Choices For Healthier Living',
                    date:'By admin | March 25th, 2019'
                },
                {
                    image:'https://avada.website/food/wp-content/uploads/sites/118/2019/03/fi-water-side-rest.jpg',
                    title:'5 Waterside Restaurants in Istanbul for Special Events',
                    date:'By admin | March 25th, 2019'
                },
            ]
        }
    },
}
</script>
<style lang="scss" scoped>
@use '../../styles/partials/mixin' as *; 
@use '../../styles/partials/variables' as *;

.image-wrapper{
    display: flex;
    flex-wrap: wrap;
    width: 70%;
}
.right-wrapper-posts{
    width: 30%;
    height: 100%;
    display: flex;
    flex-direction: column;
}
.form-control{
    padding: 1rem;
    width: 330px;
    border: none;
}
form{
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
.load-posts{
    width: 93%;
    border: none;
    padding: 1.2rem;
    background-color: #eaeae1;
    color: $darkGrey;
}
.socials-box p{
    color: $orange;
    font-size: 1.1rem;
    margin: 2rem 0;
    font-family: 'VidaLoka';
}
.socials-icon{
      height: 35px;
      margin-right: 0.8rem;
      color: $darkGrey;
      background-color: #dfdfdd;
      border-radius: 0.25rem;
    }
    .chat-box{
        display: flex;
        flex-direction: column;
    }
    .upper-box-chat{
        font-family: 'VidaLoka';
        padding: 2rem;
        margin: auto;
        font-size: 1.2rem;
    }
    .divider{
        height: 45px;
        border: 0.5px solid black;
    }

    .comment{

        display: flex;

        img{
            height: 60px;
            width: 60px;
        }

        .detail-comment{
            color: black;
            font-family: 'Catamaran', sans-serif;
            font-weight: 200;
        }
        .date{
            color: $darkGrey;
            font-family: 'Catamaran', sans-serif;
            font-size: 0.85rem;
        }
    }

    .twitter-box{
        background-color: white;
        height: 600px;
        border-radius: 0.5rem;
    }

</style>