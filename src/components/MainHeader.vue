<template>
    <header id="main-header">
        <nav class="container">
            <figure>
                <a href="#">
                    <img src="../assets/img/dc-logo.png" alt="DC Comics Logo">
                </a>
            </figure>

            <ul>
                <li v-for="item in menuItems" :key="item.key">
                    <a :href="item.url" :class="{ 'active': item.current }">{{ item.text }}</a>
                </li>
            </ul>
        </nav>
    </header>
</template>

<script>

export default {
    name: 'MainHeader',
    data() {
        return {
            menuItems: [
                {
                    text: 'Characters',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Comics',
                    url: '#',
                    current: true,
                },
                {
                    text: 'Movies',
                    url: '#',
                    current: false,
                },
                {
                    text: 'TV',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Games',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Collectibles',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Videos',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Fans',
                    url: '#',
                    current: false,
                },
                {
                    text: 'News',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Shop',
                    url: '#',
                    current: false,
                },
            ],
        }
    }
}

</script>

<style lang="scss" scoped>
@import '../assets/sass/vars';

#main-header {
    nav {
        padding: 20px 0;
        font-size: 12px;
        font-weight: 700;
        text-transform: uppercase;
    }

    nav,
    ul {
        display: flex;
        justify-content: space-between;
        align-items: center;
    }

    img {
        height: 80px;
        display: block;
    }

    ul li {
        margin: 0 15px;

        a {
            position: relative;

            &.active,
            &:hover {
                color: $primary_color;
            }

            &:hover::after,
            &.active::after {
                content: '';
                width: 100%;
                height: 6px;
                background-color: $primary_color;
                position: absolute;
                bottom: calc(-60px + 50%);
                left: 0;
            }
        }
    }
}
</style>