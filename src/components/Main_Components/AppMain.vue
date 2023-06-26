<template>
  <AppJumbotron/>
  <AppFoodieJournal/>
  </template>
  <script>
  import AppJumbotron from '../Main_Components/AppJumbotron.vue';
  import AppFoodieJournal from './AppFoodieJournal.vue';
  export default {
    name:"AppMain",
    components:{
      AppJumbotron,
      AppFoodieJournal,
    }
  }
  </script>
  <style lang="scss" scoped>
  
  </style>