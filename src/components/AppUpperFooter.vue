<script>
    export default {
        name: "AppUpperFooter",
        data() {
            return {
                footerLinks: [
                    {
                        title: "DC COMICS",
                        links: [
                            { name: "Characters", href: "#" },
                            { name: "Comics", href: "#" },
                            { name: "Movies", href: "#" },
                            { name: "TV", href: "#" },
                            { name: "Games", href: "#" },
                            { name: "Videos", href: "#" },
                            { name: "News", href: "#" }
                        ]
                    },
                    {
                        title: "SHOP",
                        links: [
                            { name: "Shop DC", href: "#" },
                            { name: "Shop DC Collectibles", href: "#" }
                        ]
                    },
                    {
                        title: "DC",
                        links: [
                            { name: "Terms of Use", href: "#" },
                            { name: "Privacy Policy (New)", href: "#" },
                            { name: "Ad Choices", href: "#" },
                            { name: "Advertising", href: "#" },
                            { name: "Jobs", href: "#" },
                            { name: "Subscriptions", href: "#" },
                            { name: "Talent Workshops", href: "#" },
                            { name: "CPSC Certificates", href: "#" },
                            { name: "Ratings", href: "#" },
                            { name: "Shop Help", href: "#" },
                            { name: "Contacts Us", href: "#" }
                        ]
                    },
                    {
                        title: "SITES",
                        links: [
                            { name: "DC", href: "#" },
                            { name: "MAD Magazine", href: "#" },
                            { name: "DC Kids", href: "#" },
                            { name: "DC Universe", href: "#" },
                            { name: "DC Power Visa", href: "#" }
                        ]
                    }
                ]
            }
        }
    }
</script>


<template>

    <div class="up_foot_cont">
        <div class="container">
            <div class="foot_menu" v-for="(link, index) in footerLinks" :key="index">
                <h5>{{ link.title }}</h5>
                <ul>
                    <li v-for="(ref, index) in link.links" :key="index">
                        <a :href="ref.href">{{ ref.name }}</a>
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