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
            <img :src="comic.thumb" alt="series + 'image'">
        </div>
        <p>{{ comic.series }}</p>
        <p>{{ comic.price }}</p>
    </div>
</template>



<style scoped>
.card {
    color: var(--light-header);

    & .cont-img {
        width: 150px;
        height: 150px;
        margin-top: 2rem;
        overflow: hidden;

        & img {
            max-width: 100%;
        }
    }

    & p {
        font-size: small;
        font-weight: 100;
        line-height: 1rem;
        padding-top: 0.25rem;
        padding-bottom: rem;
    }


    /*poteva essere anche cosí per sistemare limagine e che siano rettangolari:display: 
    width: 100%;
    object-fit: cover
    object-position: top (per alineare) */
}
</style>