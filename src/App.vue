<template>
  <div id="app">
    <MainHeader />
    <MainContent />
    <MainFooter />
  </div>
</template>

<script>
import MainHeader from './components/MainHeader.vue';
import MainContent from './components/MainContent.vue';
import MainFooter from './components/MainFooter.vue';

export default {
  name: 'App',
  components: {
    MainHeader,
    MainContent,
    MainFooter,
  },
}
</script>

<style>
* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}

body {
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
}

img {
  max-width: 100%;
  height: auto;
}

a {
  text-decoration: none;
  color: #000;
}

ul {
  list-style-type: none;
}

ul li {
  padding: 0;
}

.container {
  margin: 0 auto;
  max-width: 1200px;
}
</style>