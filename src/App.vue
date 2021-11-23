<template>
  <div id="app">
    <!-- Header -->
    <Header />

    <!-- Main -->
    <Main />

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
import Social from './components/Social.vue'


export default {
  name: 'App',
  components: {
    Header,
    Main,
    Footer,
    Social
  }
}
</script>

<style lang="scss">
@import '@/styles/utilities';
@import '@/styles/variables';


</style>
