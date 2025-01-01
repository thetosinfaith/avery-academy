<template>
  <div>
    <MainNavbar />
    <HeroSection />
    <OfferSection/>
  </div>
</template>

<script>

import MainNavbar from './components/MainNavbar.vue';
import HeroSection from './components/HeroSection.vue';
import OfferSection from './components/OfferSection.vue';

export default {
  name: 'App',
  components: {
    MainNavbar,
    HeroSection,
    OfferSection,
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
