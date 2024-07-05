<script>
    export default {
        name: "AppUpperFooter",
    }
</script>


<template>

    <div class="up_foot_cont">
        <div class="container">
            <div class="foot_menu">
                <h5>Titolo</h5>
                <ul>
                    <li>
                        <a href="#">Voce</a>
                    </li>
                    <li>
                        <a href="#">Voce</a>
                    </li>
                    <li>
                        <a href="#">Voce</a>
                    </li>
                </ul>
            </div>
            <div class="foot_menu">
                <h5>Titolo</h5>
                <ul>
                    <li>
                        <a href="#">Voce</a>
                    </li>
                    <li>
                        <a href="#">Voce</a>
                    </li>
                    <li>
                        <a href="#">Voce</a>
                    </li>
                </ul>
            </div>
            <div class="foot_menu">
                <h5>Titolo</h5>
                <ul>
                    <li>
                        <a href="#">Voce</a>
                    </li>
                    <li>
                        <a href="#">Voce</a>
                    </li>
                    <li>
                        <a href="#">Voce</a>
                    </li>
                </ul>
            </div>
        </div>
    </div>

</template>


<style lang="scss" scoped>
    @use '../styles/partials/variables' as *;
    @use '../styles/partials/mixins' as *;

    .up_foot_cont {
        background-image: url(../assets/dc-logo-bg.png), url(../assets/footer-bg.jpg);
        background-size: 30%, cover;
        background-position-x: 75%;
        background-position-y: center;
        background-repeat: no-repeat;
        
        /* DEBUG */
        height: 250px;

        .container {
            display: flex;
            gap: 40px;
            padding: 25px 0;

            h5 {
                font-size: 18px;
                font-weight: 600;
                color: white;
                margin-bottom: 10px
            }

            ul {
                list-style-type: none;

                li a {
                    font-size: 12px;
                    color: rgb(197, 196, 196);
                }
            }
        }
    }
</style>