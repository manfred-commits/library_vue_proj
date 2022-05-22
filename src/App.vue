<template>
  <MainHeader/>
  <MainSlider/>
  <MainFooter/>
</template>

<script>
import MainHeader from './components/MainHeader.vue';
import MainSlider from './components/MainSlider.vue';
import MainFooter from './components/MainFooter.vue';


export default {
  name: 'App',
  components: {
    MainHeader,
    MainSlider,
    MainFooter
}
}
</script>

<style>

@import url('https://fonts.googleapis.com/css2?family=Roboto+Mono:wght@100;300;400;500;600;700&display=swap');


*{
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}
body{
  font-family: 'Roboto Mono', monospace;
  background-color: #1f1f22!important;
}
</style>
