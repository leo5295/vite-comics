<script>
export default {
  data() {
      return {
          menu: [
              {
                  label: 'CHARACTERS',
                  url: '#',
                  active: false
              },
              {
                  label: 'COMICS',
                  url: '#',
                  active: true
              },
              {
                  label: 'MOVIES',
                  url: '#',
                  active: false
              },
              {
                  label: 'TV',
                  url: '#',
                  active: false
              },
              {
                  label: 'GAMES',
                  url: '#',
                  active: false
              },
              {
                  label: 'COLLECTIBLES',
                  url: '#',
                  active: false
              },
              {
                  label: 'VIDEOS',
                  url: '#',
                  active: false
              },
              {
                  label: 'FANS',
                  url: '#',
                  active: false
              },
              {
                  label: 'NEWS',
                  url: '#',
                  active: false
              },
              {
                  label: 'SHOP',
                  url: '#',
                  active: false
              },
          ]
      }
  },
  methods: {
    setActive: function(index) {
      this.menu.forEach((item, i) => {
        item.active = i === index;
      });
    }
  }
}
</script>


<template lang="">
  <header>
     <a href="/" class="brand">
        <img class="logo" src="../assets/img/dc-logo.png" alt="">
     </a>
     <nav>
      <ul>
        <li v-for="(item, index) in menu" :key="index" :class="item.active ? 'active' : ''" @click="setActive(index)">
              <a :href="item.url" class="link">
              {{item.label}}
              </a>
          </li>
      </ul>
     </nav>
  </header>
</template>


<style scoped lang="scss">
header{
    height: 100px;
    display: flex;
    align-items: center;
    background-color: #fff;
}

header > a{
    width: 30%;
    text-align: center;
}

nav{
    width: 70%;
    text-align: center;
    font-size: 15px;

}
.logo{
    height: 70px;
}

ul{
    list-style: none;
}

li.active{
        border-bottom-color: #0282f9;
}

li{
    display: inline;
    a:link { text-decoration: none; }
    padding: 15px;
    border-bottom: 5px solid transparent;
    
    &:hover {
        border-bottom-color: #0282f9;
    }
}

</style>