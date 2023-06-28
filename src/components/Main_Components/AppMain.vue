<template>
  <AppJumbotron/>
  <AppFoodieJournal/>
  <AppPopularRecipes/>
  <AppCulinary/>
  <AppFarm/>
  <AppPosts/>
  </template>
  <script>
  import AppJumbotron from '../Main_Components/AppJumbotron.vue';
  import AppFoodieJournal from './AppFoodieJournal.vue';
  import AppPopularRecipes from './AppPopularRecipes.vue';
  import AppCulinary from './AppCulinary.vue';
  import AppFarm from './AppFarm.vue';
  import AppPosts from './AppPosts.vue';
  export default {
    name:"AppMain",
    components:{
      AppJumbotron,
      AppFoodieJournal,
      AppPopularRecipes,
      AppCulinary,
      AppFarm,
      AppPosts
    }
  }
  </script>
  <style lang="scss" scoped>
  
  </style>