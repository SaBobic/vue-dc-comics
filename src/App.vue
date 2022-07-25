<template>
  <div id="app">
    <MainHeader />
    <main>
      <JumbSection />
      <SeriesSection />
      <TabsSection />
    </main>
    <MainFooter />
  </div>
</template>

<script>
import MainHeader from './components/MainHeader.vue';
import TabsSection from './components/TabsSection.vue';
import JumbSection from './components/JumbSection.vue';
import SeriesSection from './components/SeriesSection.vue';
import MainFooter from './components/MainFooter.vue';

export default {
  name: 'App',
  components: {
    MainHeader,
    TabsSection,
    JumbSection,
    SeriesSection,
    MainFooter,
  },
}
</script>

<style lang="scss">
@import './assets/sass/style.scss';
</style>