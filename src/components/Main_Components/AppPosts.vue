<template>
       <div class="container">
        <div class="image-wrapper">
            <AppSinglePost class="d-flex flex-wrap" v-for="post in listPosts"
            :image="post.image"
            :title="post.title"
            :date="post.date"
            />
        </div>
   <nav class="navbar bg-body-tertiary">
  <div class="container-fluid">
    <form class="d-flex" role="search">
      <input class="form-control me-2" type="search" placeholder="Search" aria-label="Search">
    </form>
  </div>
    </nav>
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
}

</style>