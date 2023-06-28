<template>
  <AppJumbotron/>
  <AppFoodieJournal/>
  <AppPopularRecipes/>
  <AppCulinary/>
  <AppFarm/>
  <AppPosts/>
  <AppSubscribe/>
  <AppCardLower/>
  </template>
  <script>
  import AppJumbotron from '../Main_Components/AppJumbotron.vue';
  import AppFoodieJournal from './AppFoodieJournal.vue';
  import AppPopularRecipes from './AppPopularRecipes.vue';
  import AppCulinary from './AppCulinary.vue';
  import AppFarm from './AppFarm.vue';
  import AppPosts from './AppPosts.vue';
  import AppSubscribe from './AppSubscribe.vue';
  import AppCardLower from './AppCardLower.vue'
  export default {
    name:"AppMain",
    components:{
      AppJumbotron,
      AppFoodieJournal,
      AppPopularRecipes,
      AppCulinary,
      AppFarm,
      AppPosts,
      AppSubscribe,
      AppCardLower
    }
  }
  </script>
  <style lang="scss" scoped>
  
  </style>