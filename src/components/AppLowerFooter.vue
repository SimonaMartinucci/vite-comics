<script>
    export default {
        name: "AppLowerFooter",
    }
</script>


<template>
    <div class="low_foot_cont">
        <div class="container">
            <div class="sign">
                <a href="#">SIGN-UP NOW</a>
            </div>
            <div class="socials">
                <a href="#">FOLLOW US</a>
                <div class="icons">
                    <img src="../assets/footer-facebook.png" alt="">
                </div>
                <div class="icons">
                    <img src="../assets/footer-facebook.png" alt="">
                </div>
                <div class="icons">
                    <img src="../assets/footer-facebook.png" alt="">
                </div>
            </div>
        </div>
    </div>
</template>


<style lang="scss" scoped>
    @use '../styles/partials/variables' as *;
    @use '../styles/partials/mixins' as *;

    .low_foot_cont {
        background-color: $light_gray;
        height: 100px;

        .container {
            display: flex;
            justify-content: space-between;
            height: 100%;

            .sign {
                align-content: center;

                a {
                    color: white;
                    font-size: 16px;
                    font-weight: 500;
                    padding: 10px;
                    border: 3px solid $light_blue;
                }
            }

            .socials {
                display: flex;
                align-items: center;
                gap: 15px;

                a {
                    color: $light_blue;
                    font-size: 16px;
                    font-weight: 500;
                    margin-right: 10px;
                }

                .icons {
                    width: 30px;

                    img {
                        width: 100%;
                    }
                }

                .icons:hover {
                    cursor: pointer;
                }
            }
        }
    }


</style>