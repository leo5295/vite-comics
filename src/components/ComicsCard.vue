<script>
export default {
    props: {
        comic: Object
    }
}
</script>
<template lang="">
    <div class="container">
        <div class="comics-card" >
                    <div class="thumb-container">
                        <img :src="comic.thumb" :alt="comic.series" class="thumb">
                    </div>
                    <div class="title-container">
                        <h4>{{ comic.series }}</h4>
                    </div>
                </div>
    </div>
</template>
<style lang="scss" scoped>
.container {
    width: calc(100% / 6);
    padding-bottom: 5em;

    .comics-card {
        margin: 10px 0px 50px 0px;
        width: 200px;
        height: 200px;

        .thumb-container {
            width: 100%;
            height: 100%;

            .thumb {
                height: 100%;
                width: 100%;
                object-fit: cover;
                object-position: top;
            }
        }
    }

    .title-container {
        object-position: top;
        object-fit: cover;
        text-align: center;
        color: white;
        padding: 5px;
        text-transform: uppercase;
    }
}
</style>