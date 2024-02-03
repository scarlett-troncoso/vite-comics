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
        <h5>{{ comic.series }}</h5>
        <span>{{ comic.price }}</span>
    </div>
</template>



<style scoped>
.card {

    & .cont-img {
        width: 150px;

        & img {
            max-width: 100%;
        }

    }
}
</style>