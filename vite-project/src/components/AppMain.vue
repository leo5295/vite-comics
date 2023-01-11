    
<script>
    
    export default {
      data() {
          return {
              menu: [
                  {
                      label: 'DIGITAL COMICS',
                      url: '../src/assets/img/buy-comics-digital-comics.png',
                  },
                  {
                      label: 'DC MERCHANDISE',
                      url: '../src/assets/img/buy-comics-merchandise.png',
                  },
                  {
                      label: 'SUBSCRIPTION',
                      url: '../src/assets/img/buy-comics-shop-locator.png',
                  },
                  {
                      label: 'COMIC SHOP LOCATOR',
                      url: '../src/assets/img/buy-comics-subscriptions.png',
                  },
                  {
                      label: 'DC POWER VISA',
                      url: '../src/assets/img/buy-dc-power-visa.svg',
                  },
              ]
          }
      }
    }
    
</script>

<template lang="">
    <main>
        <div class="black">
            CONTENT GOES HERE
        </div>
        <div class="blue">
        <ul>
            <li v-for="(item, index) in menu" :key="index">
              <a :href="item.url" class="link">
              {{item.label}}
              </a>
              <img :src="item.url" alt="option" class="icon">
          </li>
      </ul>
        </div>
    </main>
</template>

<style lang="scss" scoped>

ul{
    display: flex;
}

.blue{    
    background-color: #0282f9;
}
.icon{
    height: 50px;
}
.black{
    height: 50px;
    width: 80%;
    margin: 0 auto;
    display: flex;
    align-items: center;
}

main{
    background-color: black;
    color: white;
}
</style>
