<template>
    <section id="main-footer-top">
        <div class="container">
            <nav>
                <div>
                    <h4>{{ footerMenuItems[0].title }}</h4>
                    <ul>
                        <li v-for="(item, i) in footerMenuItems[0].items" :key="i"><a :href="item.url">{{ item.anchor
                        }}</a></li>
                    </ul>
                    <h4>{{ footerMenuItems[1].title }}</h4>
                    <ul>
                        <li v-for="(item, i) in footerMenuItems[1].items" :key="i"><a :href="item.url">{{ item.anchor
                        }}</a></li>
                    </ul>
                </div>
                <div>
                    <h4>{{ footerMenuItems[2].title }}</h4>
                    <ul>
                        <li v-for="(item, i) in footerMenuItems[2].items" :key="i"><a :href="item.url">{{ item.anchor
                        }}</a></li>
                    </ul>
                </div>
                <div>
                    <h4>{{ footerMenuItems[3].title }}</h4>
                    <ul>
                        <li v-for="(item, i) in footerMenuItems[3].items" :key="i"><a :href="item.url">{{ item.anchor
                        }}</a></li>
                    </ul>
                </div>
            </nav>
        </div>
    </section>
</template>

<script>
export default {
    name: 'MainFooterTop',
    props: {
        footerMenuItems: Array
    }
}
</script>

<style lang="scss" scoped>
@import '../assets/sass/mixins';

#main-footer-top {
    @include bg-image('../assets/img/footer-bg.jpg');
    background-size: cover;


    nav {
        padding: 35px 0;
        @include bg-image('../assets/img/dc-logo-bg.png');
        background-position: right;
        display: flex;

        div {
            margin-right: 50px;
        }
    }

    h4,
    ul {
        margin-bottom: 15px;
    }

    h4 {
        color: #fff;
        font-size: 20px;
    }


    a {
        color: #A8A8A8;
        font-size: 12px;
    }
}
</style>