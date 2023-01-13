    
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
                <img :src="item.url" alt="option" class="icon">
              <a :href="item.url" class="link">
              {{item.label}}
              </a>
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
    height: 100px;
    display: flex;
    justify-content: center;
    align-items: center;
    align-content: space-between;
    text-align: center;
}
.icon{
    height: 60px;
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

li{
    list-style: none;
    display: flex;
    align-items: center;
}

li:last-child img{
    width: 70px;
}

a{
    margin: 10px;
    text-decoration: none;
    color: white;

}

.link:hover{
    color: inherit;
}

</style>
