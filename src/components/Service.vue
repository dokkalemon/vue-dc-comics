<template>
  <section class="service full-width">
      <div class="service-conteiner conteiner px-15">
          <div class="service-item" v-for="(item, index) in serviceItem" :key="`serviceItem-${index}`">
              <img :src="item.img" alt="">
              <h5>{{item.text}}</h5>
          </div>
          


          
      </div>

  </section>
</template>

<script>
export default {
    name: 'Service',

    data() {
        return {
            serviceItem: [
                {
                    text: 'DIGITAL COMICS',
                    img: './../assets/buy-comics-digital-comics.png'
                },
                {
                    text: 'DC MERCHANDISE',
                    img: '../assets/buy-comics-merchandise.png'
                },
                {
                    text: 'SUBSCRIPTION',
                    img: '../assets/buy-comics-subscriptions.png'
                },
                {
                    text: 'COMIC SHOP LOCATOR',
                    img: '../assets/buy-comics-shop-locator.png'
                },
                {
                    text: 'DC POWER VISA',
                    img: '../assets/buy-dc-power-visa.svg'
                },
            ]
        }
    }
}
</script>

<style lang="scss">
@import '@/styles/variables';

.service {
    background-color: $primary-color;
    .service-conteiner{
        display: flex;
        
        .service-item {
            width: calc(100% / 5);
            display: flex;
            justify-content: center;
            align-items: center;
            img {
                height: 40%;
                margin-right: 15px;
            }
            h5 {
                font-family: 'Arial', sans-serif;
                color: white;
                font-weight: 100;
                font-size: 14px;
            }
        }

    }
}




</style>