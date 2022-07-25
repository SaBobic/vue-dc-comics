<template>
    <div class="col">
        <figure>
            <div>
                <img :src="serieSrc" :alt="serieTitle">
            </div>
            <figcaption>{{ serieTitle }}</figcaption>
        </figure>
    </div>
</template>

<script>
export default {
    name: 'SerieCol',
    props: {
        serieSrc: String,
        serieTitle: String,
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