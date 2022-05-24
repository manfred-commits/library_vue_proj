<template>
  <MainHeader/>
  <main>
    <MainSlider/>
    <MainPostsSection/>
  </main>
  <MainFooter/>
</template>

<script>
import MainHeader from './components/MainHeader.vue';
import MainSlider from './components/MainSlider.vue';
import MainFooter from './components/MainFooter.vue';
import MainPostsSection from './components/MainPostsSection.vue';


export default {
  name: 'App',
  components: {
    MainHeader,
    MainSlider,
    MainFooter,
    MainPostsSection
}
}
</script>

<style lang="scss">

@import url('https://fonts.googleapis.com/css2?family=Roboto+Mono:wght@100;300;400;500;600;700&display=swap');


*{
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}
body{
  font-family: 'Roboto Mono', monospace;
  background-color: #1f1f22!important;
  main {
    width: 80%;
    margin: auto;
    padding-top: 5%;
    color: white;

    #carouselExampleCaptions {
        img {
            height: 500px;
            object-fit: cover;
        }
    }

    .card_container {
        width: 100%;
        padding: 1rem 0 1rem;

        img {
            height: 300px;
            object-fit: cover;
        }
    }
    .card{
        background-color: rgb(20, 20, 20) !important;
    }
    .card-body{
        background-color: rgb(20, 20, 20) !important;
        border: 0;
    }

}
}
</style>
