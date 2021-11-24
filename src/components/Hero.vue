<template>
  <section class="hero full-width">
      <img src="@/assets/jumbotron.jpg" alt="">
  </section>
</template>

<script>
export default {
    name: 'Hero'
}
</script>

<style lang="scss">
    .hero {
        height: 100vh;
        img {
            height: 100%;
            width: 100%;
            object-fit: cover;
        }
        
    }
</style>