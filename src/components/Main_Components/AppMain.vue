<template>
  <AppJumbotron/>
  <AppFoodieJournal/>
  <AppPopularRecipes/>
  </template>
  <script>
  import AppJumbotron from '../Main_Components/AppJumbotron.vue';
  import AppFoodieJournal from './AppFoodieJournal.vue';
  import AppPopularRecipes from './AppPopularRecipes.vue';
  export default {
    name:"AppMain",
    components:{
      AppJumbotron,
      AppFoodieJournal,
      AppPopularRecipes
    }
  }
  </script>
  <style lang="scss" scoped>
  
  </style>