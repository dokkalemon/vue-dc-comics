<template>
  <div class="series ">
      <div class="series-img ">
          <img :src="thumb" alt="">
      </div>
      <h4>{{ series }}</h4>
  </div>
</template>

<script>
export default {
    name: 'Series',

    props: {
        thumb: String,
        series: String,
    }
}
</script>

<style lang="scss">
.series {
    width: calc(100% / 6);
    padding: 0 10px;
    margin-bottom: 30px;
    
    .series-img {
        width: 100%;
        height: 190px;
        img {
            height: 100%;
            width: 100%;
            object-fit: cover;
        }
    }
    h4 {
        color: white;
        padding: 10px 0;
        font-weight: 500;
        text-transform: uppercase
    }
    

}

</style>