<script>
export default {
    name: 'AppHeader',
}
</script>

<template>
    <header>
        <div class="container d-flex">
            <div class="logoHeader">
                <img src="/img/dc-logo.png" alt="">
            </div>

            <nav>
                <ul class="mainMenu d-flex">
                    <li><a href="">CHARACTERS</a></li>
                    <li><a href="">COMICS</a></li>
                    <li><a href="">MOVIES</a></li>
                    <li><a href="">TV</a></li>
                    <li><a href="">GAMES</a></li>
                    <li><a href="">COLLECTIBLES</a></li>
                    <li><a href="">VIDEOS</a></li>
                    <li><a href="">FANS</a></li>
                    <li><a href="">NEWS</a></li>
                    <li><a href="">SHOP</a></li>
                </ul>
            </nav>
        </div>
    </header>
</template>

<style scoped>
header {
    background-color: var(--light-header);

    & img {
        width: 4rem;
    }

    & .logoHeader {
        width: 40%;
    }

    & .container {
        justify-content: space-between;
        padding: 1rem;
        align-items: center;
    }

    & .mainMenu {
        list-style: none;
        font-size: 0.65rem;
        font-weight: 700;

        & li {
            padding: 0.75rem;
        }

        & a {
            text-decoration: none;
        }
    }
}
</style>