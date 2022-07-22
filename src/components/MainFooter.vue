<template>
    <footer id="main-footer">
        <MainFooterTop />
        <MainFooterBottom />
    </footer>
</template>

<script>
import MainFooterBottom from './MainFooterBottom.vue'
import MainFooterTop from './MainFooterTop.vue'

export default {
    name: 'MainFooter',
    components: {
        MainFooterBottom,
        MainFooterTop,
    }
}
</script>

<style scoped>
</style>