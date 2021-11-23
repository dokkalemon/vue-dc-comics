<template>
    <footer class="full-width">
       <div class="footer full-width debug">
           <img src="@/assets/footer-bg.jpg" alt="">
       </div>
       <div class="footer-button">

       </div>
    </footer>






</template>




<script>
export default {
    name: 'Footer'
}
</script>





<style lang="scss">
@import '@/styles/variables';

footer {
    height: 500px;

    .footer {
        height: 100%;

        img {
            width: 100%;
            object-fit: cover;
        }
    }


    .footer-button {
        height: 150px;
        background-color: $secondary-color
    }

   
}


</style>