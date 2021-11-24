<template>
  <div id="app">
    <!-- Header -->
    <Header />

    <!-- Hero -->
    <Hero />

    <!-- Hero -->
    <Label title="Current Series"/>
    

    <!-- Main -->
    <Main />

    <!-- Service -->
    <Service />

    <!-- Footer -->
    <Footer />

    <!-- Social -->
    <Social />
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Main from './components/Main.vue'
import Footer from './components/Footer.vue'
import Service from './components/Service.vue'
import Social from './components/Social.vue'
import Hero from './components/Hero.vue'
import Label from './components/Label.vue'


export default {
  name: 'App',
  components: {
    Header,
    Main,
    Footer,
    Social,
    Service,
    Hero,
    Label
  }
}
</script>

<style lang="scss">
@import '@/styles/utilities';
@import '@/styles/variables';


</style>
