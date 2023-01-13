<script>
export default {
    data() {
        return {
            socialArray: [
                {
                    name: "facebook",
                    url: "../src/assets/img/footer-facebook.png"
                },
                {
                    name: "twitter",
                    url: "../src/assets/img/footer-twitter.png"
                },
                {
                    name: "youtube",
                    url: "../src/assets/img/footer-youtube.png"
                },
                {
                    name: "pinterest",
                    url: "../src/assets/img/footer-pinterest.png"
                },
                {
                    name: "periscope",
                    url: "../src/assets/img/footer-periscope.png"
                },
            ]
        }
    },
    methods: {
        getImageUrl(img) {
            return new URL()
        }
}
}
</script>
<template lang="">
    <footer>
        <div class="cols container">
            <div class="col-1">

                <div class="footer-links">
                    <h4>DC COMICS</h4>
                    <nav>
                        <ul>
                            <li><a href="#">Il pastifiscio</a></li>
                            <li><a href="#">Grano</a></li>
                            <li><a href="#">Filiera</a></li>
                            <li><a href="#">100 anni di pasta</a></li>
                            <li><a href="#">Sartoria della pasta</a></li>
                        </ul>
                    </nav>
                </div>
                <div class="footer-links">
                    <h4>SHOP</h4>
                    <nav>
                        <ul>
                            <li><a href="#">Il pastifiscio</a></li>
                            <li><a href="#">Grano</a></li>
                            <li><a href="#">Filiera</a></li>
                            <li><a href="#">100 anni di pasta</a></li>
                            <li><a href="#">Sartoria della pasta</a></li>
                        </ul>
                    </nav>
                </div>

            </div>
            <div class="col-2">
                <div class="footer-links">
                    <h4>DC</h4>
                    <nav>
                        <ul>
                            <li><a href="#">Il pastifiscio</a></li>
                            <li><a href="#">Grano</a></li>
                            <li><a href="#">Filiera</a></li>
                            <li><a href="#">100 anni di pasta</a></li>
                            <li><a href="#">Sartoria della pasta</a></li>
                        </ul>
                    </nav>
                </div>
            </div>
            <div class="col-3">
                <div class="footer-links">
                    <h4>SITES</h4>
                    <nav>
                        <ul>
                            <li><a href="#">Il pastifiscio</a></li>
                            <li><a href="#">Grano</a></li>
                            <li><a href="#">Filiera</a></li>
                            <li><a href="#">100 anni di pasta</a></li>
                            <li><a href="#">Sartoria della pasta</a></li>
                        </ul>
                    </nav>
                </div>
            </div>
        </div>
        <div class="social">
            <div class="container">
                <div class="row">
                    <div class="col-sx">
                        <button>SIGN-UP NOW!</button>
                    </div>
                    <div class="col-dx">
                        <ul class="ul-social">
                            <li v-for="(item, index) in socialArray" :key="index" :class="item.active ? 'active' : ''" @click="setActive(index)">
                                <a :href="item.url" class="link">
                                    <img :src="item.url" alt="option" class="icon">
                                </a>
                            </li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
    </footer>
</template>

<style lang="scss" scoped>

.container {
    display: flex;
    flex-wrap: wrap;
}

.row{
    display: flex;
    align-items: center;
}
.col-1 {
    flex-direction: column;
}

.col-2, .col-3, .col-4 {
    flex-direction: row;
}

.footer-links{
    flex: 1;

}

footer{
    height: 300px;
    background: url(../assets/img/footer-bg.jpg)
}

.logo-footer{
    position: absolute;
    top: 0;
    right: 0;
}

.social{
    height: 100px;
    background-color: black;
}

a, h4{
    color: white;
}

.ul-social{
    display: flex;
    list-style: none;
}

.ul-social li{
    margin: 20px;
}

</style>