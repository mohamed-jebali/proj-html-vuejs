<script>
import AppHeader from './components/AppHeader.vue'
import AppMain from '../src/components/Main_Components/AppMain.vue';
import AppFooter from './components/AppFooter.vue';
import AppCopyright from './components/AppCopyright.vue';
export default{
    name: "App", 
    components: {
    AppHeader,
    AppMain,
    AppFooter,
    AppCopyright
}
}
</script>

<template>
  <AppHeader/>
  <AppMain/>
  <AppFooter/>
  <AppCopyright/>
</template>

<style lang="scss">
@import "./bootstrap/scss/bootstrap";
@import url('https://fonts.googleapis.com/css2?family=Catamaran:wght@100;200;300;400;500;600;700;800;900&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Vidaloka&display=swap');

body{
  font-family: 'Catamaran', sans-serif;
  background-color: #f5f5f1;
}
ul{
  list-style-type: none;
}

</style>
