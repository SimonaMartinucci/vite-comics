<script>
    export default {
        name: "AppHeader",
    }
</script>


<template>
    <header>
        <div class="cont-header">
            <div class="header-logo"></div>
            <nav>
                <ul>
                    <li>
                        <a href="#">Home</a>
                    </li>
                    <li>
                        <a href="#">Home</a>
                    </li>
                    <li>
                        <a href="#">Home</a>
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

    .cont-header {
        width: 80%;
        margin: 0 auto;
        // DEBUG
        height: 100%;
        background-color: blue;
    }
}

</style>