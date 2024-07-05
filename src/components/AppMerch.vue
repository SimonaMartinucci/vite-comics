<script>
    export default {
        name: "AppMerch",
        data() {
            return {
                merchLinks: [
                    { name: "DIGITAL COMICS", img: "buy-comics-digital-comics.png" },
                    { name: "DC MERCHANDISE", img: "buy-comics-merchandise.png" },
                    { name: "SUBSCRIPTION", img: "buy-comics-subscriptions.png" },
                    { name: "COMIC SHOP LOCATION", img: "buy-comics-shop-locator.png" },
                    { name: "DC POWER VISA", img: "buy-dc-power-visa.svg" }
                ]
            }
        },
        methods: {
            getImagePath: function(img) {
                return new URL(`../assets/${img}`, import.meta.url).href;
            }
        }
    }
</script>


<template>
    <div class="merch-cont">
        <div class="container">
           <div class="item" v-for="(link, index) in merchLinks" :key="index">
                <div class="item_img">
                    <img :src='getImagePath(link.img)' :alt="link.name">
                </div>
                <div class="item_descr">{{link.name}}</div>
           </div>
        </div>
    </div>
</template>


<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;

.merch-cont {
    background-color: $light_blue;
    // DEBUG
    height: 150px;

    .container {
        display: flex;
        justify-content: space-around;
        height: 100%;

        .item {
            align-content: center;
            color: white;
            display: flex;
            align-items: center;

            .item_img {
                width: 40px;
                height: 40px;
                margin-right: 15px;

                img {
                    max-width: 100%;
                    height: 100%;
                }
            }

            .item_descr {
                font-size: 12px;
            }
        }
    }
}

</style>