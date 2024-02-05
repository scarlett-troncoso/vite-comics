<script>
export default {
    name: 'AppHeader',

    data() {
        return {
            logo: '/img/dc-logo.png',
            menuBar: [
                'CHARACTERS',
                'COMICS',
                'MOVIES',
                'TV',
                'GAMES',
                'COLLECTIBLES',
                'VIDEOS',
                'FANS',
                'NEWS',
                'SHOP'
            ]
        }
    }
}
</script>

<template>
    <header>
        <div class="container d-flex">
            <div class="logoHeader">
                <img :src="logo" alt="">
            </div>

            <nav class="d-flex">
                <ul class="mainMenu d-flex">
                    <li v-for="item in menuBar">
                        <a href="">{{ item }}</a>
                    </li>
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
        gap: 1rem;
        list-style: none;
        font-size: 0.65rem;
        font-weight: 700;

        &>li {
            padding: 0.75rem 0 0.75rem 0;
            border-bottom: 4px solid transparent;

            & a {
                text-decoration: none;
            }
        }

        &>li:hover {
            border-bottom: 4px solid var(--secondary-blue);
        }


    }
}
</style>

