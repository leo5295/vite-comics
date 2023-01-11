<script>

import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppFooter from './components/AppFooter.vue';


export default {
  components: {
    AppHeader,
    AppMain,
    AppFooter,
  }
}
</script>

<template>
  <div>
  <AppHeader />
  <AppMain />
  <AppFooter />
  </div>
</template>


<style lang="scss">
@use './styles/generals.scss' as *;

@import url('https://fonts.googleapis.com/css2?family=Roboto&display=swap');

*{
  font-family: 'Roboto', sans-serif;
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
</style>