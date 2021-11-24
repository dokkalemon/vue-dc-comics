<template>
  <div class="button full-width">
      <button class="secondary">LOAD MORE</button>
  </div>
</template>

<script>
export default {
    name: 'Button'
}
</script>

<style scoped lang="scss">

@import '@/styles/variables';



.button{
    display: flex;
    justify-content: center;
    align-items: center;
    padding: 0 0 30px 0;
    .secondary {
        background-color: $primary-color;
        width: 230px;
    }
}

</style>