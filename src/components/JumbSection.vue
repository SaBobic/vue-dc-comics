<template>
    <section class="jumbotron"></section>
</template>

<script>
export default {
    name: 'JumbSection',
}
</script>

<style lang="scss" scoped>
@import '../assets/sass/mixins';

section.jumbotron {
    height: 400px;
    @include bg-image('../assets/img/jumbotron.jpg');
}
</style>