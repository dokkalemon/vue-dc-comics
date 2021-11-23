<template>
  <div id="app">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
    <Header />
  </div>
</template>

<script>
import Header from './components/Header.vue'

export default {
  name: 'App',
  components: {
    Header
  }
}
</script>

<style lang="scss">
@import '@/styles/utilities';
@import '@/styles/variables';


</style>
