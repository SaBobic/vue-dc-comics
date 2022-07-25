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
import MainHeader from './components/MainHeader.vue';
import TabsSection from './components/TabsSection.vue';
import JumbSection from './components/JumbSection.vue';
import SeriesSection from './components/SeriesSection.vue';
import MainFooterBottom from './components/MainFooterBottom.vue';
import MainFooterTop from './components/MainFooterTop.vue';
import seriesJson from './assets/dc-comics.json';

export default {
  name: 'App',
  data() {
    return {
      seriesJson,
      mainMenuItems: [
        {
          text: 'Characters',
          url: '#',
          current: false,
        },
        {
          text: 'Comics',
          url: '#',
          current: true,
        },
        {
          text: 'Movies',
          url: '#',
          current: false,
        },
        {
          text: 'TV',
          url: '#',
          current: false,
        },
        {
          text: 'Games',
          url: '#',
          current: false,
        },
        {
          text: 'Collectibles',
          url: '#',
          current: false,
        },
        {
          text: 'Videos',
          url: '#',
          current: false,
        },
        {
          text: 'Fans',
          url: '#',
          current: false,
        },
        {
          text: 'News',
          url: '#',
          current: false,
        },
        {
          text: 'Shop',
          url: '#',
          current: false,
        },
      ],
      footerMenuItems: [
        {
          title: 'DC COMICS',
          items: [
            {
              anchor: 'Characters',
              url: '#',
            },
            {
              anchor: 'Comics',
              url: '#',
            },
            {
              anchor: 'Movies',
              url: '#',
            },
            {
              anchor: 'TV',
              url: '#',
            },
            {
              anchor: 'Games',
              url: '#',
            },
            {
              anchor: 'Videos',
              url: '#',
            },
            {
              anchor: 'News',
              url: '#',
            },
          ]
        },
        {
          title: 'SHOP',
          items: [
            {
              anchor: 'Shop DC',
              url: '#',
            },
            {
              anchor: 'Shop DC Collectibles',
              url: '#',
            },
          ]
        },
        {
          title: 'DC',
          items: [
            {
              anchor: 'Terms Of Use',
              url: '#',
            },
            {
              anchor: 'Privacy Policy',
              url: '#',
            },
            {
              anchor: 'Ad Choices',
              url: '#',
            },
            {
              anchor: 'Advertising',
              url: '#',
            },
            {
              anchor: 'Jobs',
              url: '#',
            },
            {
              anchor: 'Subscriptions',
              url: '#',
            },
            {
              anchor: 'Talent Workshops',
              url: '#',
            },
            {
              anchor: 'CPSC Certificates',
              url: '#',
            },
            {
              anchor: 'Ratings',
              url: '#',
            },
            {
              anchor: 'Shop Help',
              url: '#',
            },
            {
              anchor: 'Contact Us',
              url: '#',
            },
          ]
        },
        {
          title: 'SITES',
          items: [
            {
              anchor: 'DC',
              url: '#',
            },
            {
              anchor: 'MAD Magazine',
              url: '#',
            },
            {
              anchor: 'DC Kids',
              url: '#',
            },
            {
              anchor: 'DC Universe',
              url: '#',
            },
            {
              anchor: 'DC Power Visa',
              url: '#',
            },
          ]
        },
      ]
    };
  },
  computed: {
    series() {
      return JSON.parse(JSON.stringify(this.seriesJson));
    }
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