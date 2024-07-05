<script>
    export default {
        name: "AppProducts",
    }
</script>


<template>
    <div class="content-cont">
        <div class="container">
            <h3>-- Content goes here --</h3>>
        </div>
    </div>
</template>


<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;

.content-cont {
    background-color: #1c1c1c;
    // DEBUG
    height: 130px;

    h3 {
        color: white;
        font-size: 25px;
        padding-top: 50px;
    }
}
</style>