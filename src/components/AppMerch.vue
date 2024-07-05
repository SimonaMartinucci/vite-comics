<script>
    export default {
        name: "AppMerch",
    }
</script>


<template>
    <div class="merch-cont">
        <div class="container">
           <div class="item">
                <div class="item_img">
                    <img src="../assets/buy-comics-digital-comics.png" alt="">
                </div>
                <div class="item_descr">Prova prova</div>
           </div>
           <div class="item">
                <div class="item_img">
                    <img src="../assets/buy-comics-merchandise.png" alt="">
                </div>
                <div class="item_descr">Prova prova</div>
           </div>
           <div class="item">
                <div class="item_img">
                    <img src="../assets/buy-comics-shop-locator.png" alt="">
                </div>
                <div class="item_descr">Prova prova</div>
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
                height: 50px;
                margin-right: 15px;

                img {
                    height: 100%;
                }
            }
        }
    }
}

</style>