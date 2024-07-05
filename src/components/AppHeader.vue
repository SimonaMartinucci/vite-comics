<script>
    export default {
        name: "AppHeader",
    }
</script>


<template>
    <header>
        <div class="cont-header">
            <div class="header-logo">
                <img src="../assets/dc-logo.png" alt="logo">
            </div>
            <nav>
                <ul>
                    <li>
                        <a href="#">HOME</a>
                    </li>
                    <li class="active">
                        <a href="#">HOME</a>
                    </li>
                    <li>
                        <a href="#">HOME</a>
                    </li>
                </ul>
            </nav>
        </div>
    </header>
</template>


<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;

header {
    width: 100%;
    background-color: white;
    height: 100px;

    a {
        text-decoration: none;
        color: $light_gray;
    }    

    .cont-header {
        width: 70%;
        height: 100%;
        margin: 0 auto;
        display: flex;
        justify-content: space-between;
        align-items: center;

        .header-logo {
        width: 80px;

            img {
                max-width: 100%;
            }
        }

        nav {
            height: 100%;

            ul {
            list-style-type: none; 
            display: flex;
            // gap: 15px;
            height: 100%;

                li {
                    height: 100%;
                    align-content: center;
                    padding: 0 15px;
                }

                li:hover {
                    background-color: rgb(239, 238, 238);
                    cursor: pointer;
                }

                li.active {
                    border-bottom: 3px solid $light_blue;
                }

                li.active a {
                    color: $light_blue;
                }
            }
        }
    }       
}

</style>