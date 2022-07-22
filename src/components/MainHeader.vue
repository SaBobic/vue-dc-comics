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

<style scoped>
#main-header nav {
    padding: 20px 0;
    font-size: 12px;
    font-weight: 700;
    text-transform: uppercase;
}

#main-header nav,
#main-header ul {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

#main-header img {
    height: 80px;
    display: block;
}

#main-header ul li {
    margin: 0 15px;
}

#main-header ul li a {
    position: relative;
}

#main-header ul li a.active,
#main-header ul li a:hover {
    color: #0282F9;
}

#main-header ul li a:hover::after,
#main-header ul li a.active::after {
    content: '';
    width: 100%;
    height: 6px;
    background-color: #0282F9;
    position: absolute;
    bottom: calc(-60px + 50%);
    left: 0;
}
</style>