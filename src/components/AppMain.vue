<script>
export default {
    name: 'AppMain',
}
</script>

<template>
    <main>
        <div class="content-here container">
            <h3><a href="#"> - - > Content goes here < - - </a>
            </h3>
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