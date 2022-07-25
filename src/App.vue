<template>
  <div id="app">
    <MainHeader />
    <main>
      <JumbSection />
      <FilmsSection />
      <TabsSection />
    </main>
    <MainFooter />
  </div>
</template>

<script>
import MainHeader from './components/MainHeader.vue';
import TabsSection from './components/TabsSection.vue';
import JumbSection from './components/JumbSection.vue';
import FilmsSection from './components/FilmsSection.vue';
import MainFooter from './components/MainFooter.vue';

export default {
  name: 'App',
  components: {
    MainHeader,
    TabsSection,
    JumbSection,
    FilmsSection,
    MainFooter,
  },
}
</script>

<style lang="scss">
@import './assets/sass/style.scss';
</style>