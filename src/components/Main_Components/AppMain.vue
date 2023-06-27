<template>
  <AppJumbotron/>
  <AppFoodieJournal/>
  <AppPopularRecipes/>
  <AppCulinary/>
  <AppFarm/>
  </template>
  <script>
  import AppJumbotron from '../Main_Components/AppJumbotron.vue';
  import AppFoodieJournal from './AppFoodieJournal.vue';
  import AppPopularRecipes from './AppPopularRecipes.vue';
  import AppCulinary from './AppCulinary.vue';
  import AppFarm from './AppFarm.vue';
  export default {
    name:"AppMain",
    components:{
      AppJumbotron,
      AppFoodieJournal,
      AppPopularRecipes,
      AppCulinary,
      AppFarm
    }
  }
  </script>
  <style lang="scss" scoped>
  
  </style>