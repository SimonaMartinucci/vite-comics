<script>
    export default {
        name: "ProductCards",
        props: {
            details: Object,
        }
    }
</script>


<template>
    <div class="card">
        <div class="card-img">
            <img :src="details.thumb" :alt="details.series">
        </div>
        <h4>{{ details.series }}</h4>
    </div>
</template>


<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;

.card {
    width: calc((100% / 6) - 30px);

    h4 {
        color: white;
        font-size: 15px;
        margin: 10px 0;
    }
    
    .card-img {
        width: 150px;
        height: 150px;

        img {
            width: 100%;
            max-height: 100%;
            object-fit: cover;
            object-position: top;
        }
    }
}

</style>