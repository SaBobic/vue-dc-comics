<template>
    <section id="tabs" class="bg-primary">
        <div class="row container">
            <div v-for="item in tabsItems" class="col" :key="item.src">
                <figure>
                    <img :src="item.src" :alt="item.text">
                    <figcaption>{{ item.text }}</figcaption>
                </figure>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'TabsSection',
    data() {
        return {
            tabsItems: [
                {
                    text: 'Digital Comics',
                    src: require('../assets/img/buy-comics-digital-comics.png'),
                },
                {
                    text: 'DC Merchandise',
                    src: require('../assets/img/buy-comics-merchandise.png'),
                },
                {
                    text: 'Subscription',
                    src: require('../assets/img/buy-comics-subscriptions.png'),
                },
                {
                    text: 'Comic Shop Locator',
                    src: require('../assets/img/buy-comics-shop-locator.png'),
                },
                {
                    text: 'DC Power USA',
                    src: require('../assets/img/buy-dc-power-visa.svg'),
                },
            ],
        }
    }
}
</script>

<style lang="scss" scoped>
#tabs {
    color: #fff;

    .row {
        padding: 50px 40px;
        display: flex;

        .col {
            width: calc(100% / 5);

            figure {
                display: flex;
                align-items: center;

                img {
                    height: 50px;
                    margin-right: 15px;
                }
            }

        }
    }
}
</style>