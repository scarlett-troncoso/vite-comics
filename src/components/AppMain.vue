<script>
import AppJumbotron from './AppJumbotron.vue';
import ListCards from './ListCards.vue';

export default {
    name: 'AppMain',
    components: {
        AppJumbotron,
        ListCards,
    },
    data() {
        return {
            Products: [
                {
                    img: "/img/buy-comics-digital-comics.png",
                    text: "DIGITAL COMICS"
                },
                {
                    img: "/img/buy-comics-merchandise.png",
                    text: "DC MERCHANDISE"
                },
                {
                    img: "/img/buy-comics-subscriptions.png",
                    text: "SUBSCRIPTION"
                },
                {
                    img: "/img/buy-comics-shop-locator.png",
                    text: "COMIC SHOP LOCATOR"
                }
            ]
        }
    }
}
</script>

<template>
    <main>
        <AppJumbotron></AppJumbotron>
        <ListCards></ListCards>

        <section class="products">
            <ul class="container d-flex">

                <li class="d-flex" v-for="product in Products">
                    <div class="cont-img">
                        <img :src=product.img alt="#">
                    </div>
                    <a href="#">{{ product.text }}</a>
                </li>

                <li class="d-flex">
                    <div class="cont-img visa">
                        <img src="/img/buy-dc-power-visa.svg" alt="">
                    </div>
                    <a href="#">DC POWER VISA</a>
                </li>
            </ul>
        </section>
    </main>
</template>

<style scoped>
main {
    background-color: var(--primary-dark);

    & .products {
        background-color: var(--secondary-blue);
        padding: 1.5rem;

        & ul {
            justify-content: space-between;

            & li {
                padding: 1rem;

                & .cont-img {
                    width: 2.75rem;
                    height: 2.75rem;
                }

                & img {
                    height: 100%;
                    align-items: end;
                }

                & .visa>img {
                    width: 100%;
                }

                & a {
                    font-weight: 400;
                    font-size: 0.70rem;
                    padding: 0.75rem;
                    color: var(--light-header);
                    text-decoration: none;
                }
            }
        }
    }
}
</style>