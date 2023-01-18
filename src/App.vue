<script>

import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppFooter from './components/AppFooter.vue';
import comicsData from './assets/data/dataComics.js';
import ComicsList from './components/ComicsList.vue';
import AppJumbo from './components/AppJumbo.vue';




export default {
  components: {
    AppHeader,
    AppJumbo,
    comicsData,
    ComicsList,
    AppMain,
    AppFooter,
  }
}
</script>

<template>
  <div>
    <AppHeader />
    <AppJumbo />
    <comicsData />
    <ComicsList />

    <AppMain />
    <AppFooter />
  </div>
</template>


<style lang="scss">
@use './styles/generals.scss' as *;

@import url('https://fonts.googleapis.com/css2?family=Poppins&display=swap');


* {
  font-family: 'Poppins', sans-serif;
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
</style>