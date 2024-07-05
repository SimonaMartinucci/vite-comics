<script>
    export default {
        name: "AppHeader",
        data() {
            return {
                links: [
                    { name: "CHARACTERS", href: "#", current: false },
                    { name: "COMICS", href: "#", current: false },
                    { name: "MOVIES", href: "#", current: true },
                    { name: "TV", href: "#", current: false },
                    { name: "GAMES", href: "#", current: false },
                    { name: "COLLECTIBLES", href: "#", current: false },
                    { name: "VIDEOS", href: "#", current: false },
                    { name: "FANS", href: "#", current: false },
                    { name: "NEWS", href: "#", current: false },
                    { name: "SHOP", href: "#", current: false }
                ]
            }
        }
    }
</script>


<template>
    <header>
        <div class="container cont-header">
            <div class="header-logo">
                <img src="../assets/dc-logo.png" alt="logo">
            </div>
            <nav>
                <ul>
                    <li v-for="(link, index) in links" :key="index" :class="link.current ? 'active' : ''">
                        <a :href="link.href">{{ link.name }}</a>
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
    height: 120px;

    a {
        color: $light_gray;
    }

    .cont-header {
        height: 100%;
        display: flex;
        justify-content: space-between;
        align-items: center;

        .header-logo {
            height: 70%;

                img {
                    max-height: 100%;
                }
        }

        nav {
            height: 100%;

            ul {
            list-style-type: none; 
            display: flex;
            height: 100%;

                li {
                    height: 100%;
                    align-content: center;
                    padding: 0 15px;
                    font-size: 12px;
                }

                li:hover {
                    background-color: rgb(239, 238, 238);
                }

                li.active {
                    border-bottom: 4px solid $light_blue;
                }

                li.active a {
                    color: $light_blue;
                }
            }
        }
    }       
}

</style>