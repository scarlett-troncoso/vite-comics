<script>
export default {
    name: 'ComicsCards.vue',
    props: {
        comic: Object
    }
}
</script>

<template>
    <div class="card">
        <div class="cont-img">
            <img :src="comic.thumb" alt="">
        </div>
        <div class="titlePrice">
            <p>{{ comic.series }}</p>
            <p>{{ comic.price }}</p>
        </div>

    </div>
</template>



<style scoped>
.card {
    color: var(--light-header);

    & .titlePrice {
        font-size: small;
        font-weight: 100;
        line-height: 1rem;
        padding-top: 0.25rem;
        padding-bottom: 2rem;
    }


    & .cont-img {
        width: 150px;
        height: 150px;
        overflow: hidden;

        & img {
            max-width: 100%;
        }

    }
}
</style>