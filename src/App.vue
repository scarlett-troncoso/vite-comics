<script >
import AppHeader from './components/AppHeader.vue';

import AppMain from './components/AppMain.vue';

export default {
  name: 'App',
  components: {
    AppHeader,
    AppMain,
  }
}
</script>

<template>
  <AppHeader></AppHeader>

  <AppMain></AppMain>

  <footer>
    <section class="site-bar-footer container d-flex">
      <nav class="d-flex">
        <ul>
          <h5>DC COMICS</h5>
          <li><a href="">Chacarters</a></li>
          <li><a href="">Comics</a></li>
          <li><a href="">Movies</a></li>
          <li><a href="">TV</a></li>
          <li><a href="">Games</a></li>
          <li><a href="">Videos</a></li>
          <li><a href="">News</a></li>

          <ul>
            <h5>SHOP</h5>
            <li><a href="">Shop DC</a></li>
            <li><a href="">Shop DC Collectibles</a></li>
          </ul>
        </ul>

        <ul>
          <h5>DC</h5>
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
          <h5>SITES</h5>
          <li><a href="">DC</a></li>
          <li><a href="">MAD Magazine</a></li>
          <li><a href="">DC Kids</a></li>
          <li><a href="">DC Universe</a></li>
          <li><a href="">DC Power Visa</a></li>
        </ul>
      </nav>

      <div class="cont-img">
        <img src="/img/dc-logo-bg.png" alt="">
      </div>
    </section>

    <section class="bar-social">
      <div class="container d-flex">

        <button> SIGN-UP NOW!</button>

        <ul class="d-flex">
          <li>
            <H4>FOLLOW US</H4>
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

<style>
footer {
  background-image: url(/img/footer-bg.jpg);
  background-repeat: no-repeat;
  background-size: 100%;
  height: 300px;

  & .bar-social {
    background-color: var(--gray-footer);
  }
}
</style>
