<template>
  <section class="label conteiner px-15">
      <div class="label-conteiner">
          <h3>{{ title }}</h3>
      </div>
  </section>
</template>

<script>
export default {
    name: 'Label',

    props: {
        title: String
    }
}
</script>

<style lang="scss">
@import '@/styles/variables';

.label {
    display: flex;
    position: relative;
    top: -25px;
    
    .label-conteiner {
        background-color: $primary-color;
        padding: 10px 20px;
        h3 {
            text-transform: uppercase;
            color: white;
            font-weight: 500;
        }

    }
}

</style>