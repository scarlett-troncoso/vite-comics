<script>
export default {
    name: 'AppFooter'
}
</script>


<template>
    <footer>
        <section class="site-bar-footer container d-flex">
            <nav class="d-flex">
                <ul>
                    <h4>DC COMICS</h4>
                    <li><a href="">Chacarters</a></li>
                    <li><a href="">Comics</a></li>
                    <li><a href="">Movies</a></li>
                    <li><a href="">TV</a></li>
                    <li><a href="">Games</a></li>
                    <li><a href="">Videos</a></li>
                    <li><a href="">News</a></li>

                    <ul class="shop-ul">
                        <h4>SHOP</h4>
                        <li><a href="">Shop DC</a></li>
                        <li><a href="">Shop DC Collectibles</a></li>
                    </ul>
                </ul>

                <ul>
                    <h4>DC</h4>
                    <li><a href="">Terms Of Use</a></li>
                    <li><a href="">Privacy policy (New)</a></li>
                    <li><a href="">Ad Choices</a></li>
                    <li><a href="">Advertising</a></li>
                    <li><a href="">Jobs</a></li>
                    <li><a href="">Subscriptions</a></li>
                    <li><a href="">Talent Workshops</a></li>
                    <li><a href="">CPSC Certificates</a></li>
                    <li><a href="">Ratings</a></li>
                    <li><a href="">Shop Help</a></li>
                    <li><a href="">Contact Us</a></li>
                </ul>

                <ul>
                    <h4>SITES</h4>
                    <li><a href="">DC</a></li>
                    <li><a href="">MAD Magazine</a></li>
                    <li><a href="">DC Kids</a></li>
                    <li><a href="">DC Universe</a></li>
                    <li><a href="">DC Power Visa</a></li>
                </ul>
            </nav>

            <div class="cont-img">
                <!--<img src="/img/dc-logo-bg.png" alt="">-->
            </div>

        </section>

        <section class="bar-social">
            <div class="container d-flex">

                <button> SIGN-UP NOW!</button>

                <ul class="d-flex">
                    <li>
                        <h4>FOLLOW US</h4>
                    </li>
                    <li>
                        <img src="/img/footer-facebook.png" alt="">
                    </li>

                    <li>
                        <img src="/img/footer-twitter.png" alt="">
                    </li>

                    <li>
                        <img src="/img/footer-youtube.png" alt="">
                    </li>

                    <li>
                        <img src="/img/footer-pinterest.png" alt="">
                    </li>

                    <li>
                        <img src="/img/footer-periscope.png" alt="">
                    </li>
                </ul>
            </div>
        </section>
    </footer>
</template>


<style scoped>
footer {
    background-image: url(/img/footer-bg.jpg);
    background-repeat: no-repeat;
    background-size: 100%;
    height: 300px;

    & ul {
        list-style: none;
        padding: 1rem;
    }

    & .site-bar-footer {
        justify-content: space-between;

        & h4 {
            color: var(--light-header);
            line-height: 2rem;
        }

        & .shop-ul {
            padding-left: 0;
        }

        & li {
            line-height: 0.90rem;

            & a {
                text-decoration: none;
                color: var(--gray-main);
                font-size: 0.60rem;
            }
        }

        & .cont-img {
            background-image: url(/img/dc-logo-bg.png);
            background-size: 440px;
            background-repeat: no-repeat;
            width: 440px;
            height: 440px;
            margin: -4.5rem -4.5rem;
            margin-right: revert-layer;
        }
    }

    & .bar-social {
        background-color: var(--gray-footer);
        padding: 1.25rem;

        & div {
            justify-content: space-between;
            align-items: center;

            & button {
                height: 2.5rem;
                background-color: transparent;
                border: 2px solid var(--secondary-blue);
                padding: 0.75rem;
                color: var(--light-header);
                font-weight: 600;
            }

            & li {
                padding: 0 0.5rem 0 0.5rem;
            }

            & h4 {
                color: var(--secondary-blue);
                line-height: 2.25rem;
            }
        }
    }
}
</style>