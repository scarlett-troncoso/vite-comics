<script>
import ComicsCards from './ComicsCards.vue';
export default {
    name: 'AppMain',
    components: {
        ComicsCards
    },
    data() {
        return {
            comics: [
                {
                    thumb: "https://www.coverbrowser.com/image/action-comics/1-1.jpg",
                    price: "$19.99",
                    series: "Action Comics",
                    type: "comic book",
                },
                {
                    thumb: "https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/M/1/M1BLLA015ISBN_0.jpg",
                    price: "$3.99",
                    series: "American Vampire 1976",
                    type: "comic book",
                },
                {
                    thumb: "https://media.wired.com/photos/593384dad80dd005b42b2817/master/w_2560%2Cc_limit/Aquaman-16.jpg",
                    price: "$16.99",
                    series: "Aquaman",
                    type: "graphic novel",
                },
                {
                    thumb: "https://d29xot63vimef3.cloudfront.net/image/batgirl/1-1.jpg",
                    price: "$2.99",
                    series: "Batgirl",
                    type: "comic book",
                },
                {
                    thumb: "https://static.posters.cz/image/750/locandine-film-in-plexiglass-batman-prowl-comic-cover-i69653.jpg",
                    price: "$3.99",
                    series: "Batman",
                    type: "comic book",
                },
                {
                    thumb: "https://static.wikia.nocookie.net/marvel_dc/images/5/50/Batman_Beyond_v.1_1.jpg",
                    price: "$2.99",
                    series: "Batman Beyond",
                    type: "comic book",
                },
                {
                    thumb: "https://static.wikia.nocookie.net/marvel_dc/images/0/0d/Batman_Superman_Vol_1_1.jpg",
                    price: "$3.99",
                    series: "Batman/Superman",
                    type: "comic book",
                },
                {
                    thumb: "https://static.wikia.nocookie.net/marvel_dc/images/c/cf/Batman_Superman_Annual_Vol_2_1.jpg",
                    price: "$4.99",
                    series: "Batman/Superman Annual",
                    type: "comic book",
                },
                {
                    thumb: "https://static.wikia.nocookie.net/marvel_dc/images/5/54/Batman_The_Joker_War_Zone_Vol_1_1.jpg",
                    price: "$5.99",
                    series: "Batman: The Joker War Zone",
                    type: "comic book",
                },
                {
                    thumb: "https://static.wikia.nocookie.net/marvel_dc/images/6/64/Batman_Three_Jokers_Collected.jpg",
                    price: "$6.99",
                    series: "Batman: Three Jokers",
                    type: "comic book",
                },
                {
                    thumb: "https://static.wikia.nocookie.net/marvel_dc/images/f/f8/Batman_White_Knight_Presents_Harley_Quinn_Vol_1_1.jpg",
                    price: "$4.99",
                    series: "Batman: White Knight Presents: Harley Quinn",
                    type: "comic book",
                },
                {
                    thumb: "https://static.wikia.nocookie.net/marvel_dc/images/c/c8/Catwoman_Vol_2_1.jpg",
                    price: "$16.99",
                    series: "Catwoman",
                    type: "graphic novel",
                },
            ]
        }
    }
}
</script>

<template>
    <main>
        <div class="content-here container">
            <h3>CURRENT SERIES</h3>
            <div class="row">
                <div class="col-2" v-for="comic in comics">
                    <ComicsCards :comic="comic"></ComicsCards>
                </div>
            </div>
            <button>Load More</button>
        </div>

        <section class="products">
            <ul class="container d-flex">

                <li class="d-flex">
                    <div class="cont-img">
                        <img src="/img/buy-comics-digital-comics.png" alt="">
                    </div>
                    <a href="#">DIGITAL COMICS</a>
                </li>

                <li class="d-flex">
                    <div class="cont-img">
                        <img src="/img/buy-comics-merchandise.png" alt="">
                    </div>
                    <a href="#">DC MERCHANDISE</a>
                </li>

                <li class="d-flex">
                    <div class="cont-img">
                        <img src="/img/buy-comics-subscriptions.png" alt="">
                    </div>
                    <a href="#">SUBSCRIPTION</a>
                </li>

                <li class="d-flex">
                    <div class="cont-img">
                        <img src="/img/buy-comics-shop-locator.png" alt="">
                    </div>
                    <a href="#">COMIC SHOP LOCATOR</a>
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

    & .row {
        display: flex;
        flex-wrap: wrap;

        & .col-2 {
            width: calc(100% / 12 * 2);
        }
    }


    background-color: var(--primary-dark);

    a {
        color: var(--light-header);
        text-decoration: none;
    }

    .content-here {
        padding: 2.5rem;
    }

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
                }
            }
        }
    }
}
</style>