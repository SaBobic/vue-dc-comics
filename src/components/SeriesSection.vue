<template>
    <section class="series-list">
        <div class="container">
            <div class="label bg-primary">
                <h2>CURRENT SERIES</h2>
            </div>
            <div class="row">
                <SerieCol v-for="(serie, i) in series" :key="i" :serieSrc="serie.thumb" :serieTitle="serie.series" />
            </div>
            <button>LOAD MORE</button>
        </div>
    </section>
</template>

<script>
import './SerieCol.vue';
import SerieCol from './SerieCol.vue';
export default {
    name: "SeriesSection",
    props: {
        series: Array,
    },
    components: { SerieCol }
}
</script>

<style lang="scss" scoped>
@import '../assets/sass/vars';

.series-list {
    background-color: $secondary-color;
    color: #fff;

    .container {
        padding: 30px 0;
        position: relative;
        text-align: center;
        padding-bottom: 30px;

        .label {
            display: inline-block;
            background-color: $primary-color;
            padding: 10px 30px;
            position: absolute;
            top: 0;
            left: 0;
            transform: translateY(-50%);
        }

        .row {
            padding: 10px 0;
            display: flex;
            flex-wrap: wrap;

            .col {
                width: calc(100% / 6);
                padding: 15px;

                figure {
                    font-size: 14px;
                    text-transform: uppercase;

                    div {
                        height: 180px;
                        overflow-y: hidden;

                        img {
                            width: 100%;
                        }
                    }

                    figcaption {
                        padding: 15px 0;
                        text-align: left;
                    }
                }
            }
        }

        button {
            color: #fff;
            border: 0;
            background-color: $primary-color;
            padding: 10px 60px;
            font-size: 12px;
            font-weight: 700;
            cursor: pointer;
        }
    }
}
</style>