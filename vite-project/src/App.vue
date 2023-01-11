<script>

import AppHeader from './components/AppHeader.vue';
import AppFooter from './components/AppFooter.vue';


export default {
  components: {
    AppHeader,
    AppFooter
  }
}
</script>

<template>
  <div>
  <AppHeader />
  <AppFooter />
  </div>
</template>


<style lang="scss">
@use './styles/generals.scss' as *;

@import url('https://fonts.googleapis.com/css2?family=Roboto&display=swap');

*{
  font-family: 'Roboto', sans-serif;
}
</style>