<template>
    <div class="col">
        <figure>
            <div>
                <img :src="serie.thumb" :alt="serie.series">
            </div>
            <figcaption>{{ serie.series }}</figcaption>
        </figure>
    </div>
</template>

<script>
export default {
    name: 'SerieCol',
    props: {
        serie: Object,
    }
}
</script>

<style lang="scss" scoped>
@import '../assets/sass/vars';

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
</style>