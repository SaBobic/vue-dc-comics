<template>
  <div id="app">
    <MainHeader :main-menu-items="mainMenuItems" />
    <main>
      <JumbSection />
      <SeriesSection :series="series" />
      <TabsSection />
    </main>
    <footer>
      <MainFooterTop :footer-menu-items="footerMenuItems" />
      <MainFooterBottom />
    </footer>
  </div>
</template>

<script>
// Data
import mainMenuItems from './assets/data/data';
import series from './assets/data/dc-comics';
import footerMenuItems from './assets/data/footer-menu-items';
// Components
import MainHeader from './components/MainHeader.vue';
import TabsSection from './components/TabsSection.vue';
import JumbSection from './components/JumbSection.vue';
import SeriesSection from './components/SeriesSection.vue';
import MainFooterBottom from './components/MainFooterBottom.vue';
import MainFooterTop from './components/MainFooterTop.vue';

export default {
  name: 'App',
  data() {
    return {
      series,
      mainMenuItems,
      footerMenuItems,
    };
  },
  components: {
    MainHeader,
    TabsSection,
    JumbSection,
    SeriesSection,
    MainFooterBottom,
    MainFooterTop,
  },
}
</script>

<style lang="scss">
@import './assets/sass/style.scss';
</style>