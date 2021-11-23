<template>
    <section class="social full-width">
        <div class="social-conteiner conteiner px-15">
            <div class="social-button ">
                <button>SIGN UP NOW!</button>
            </div>
            <div class="social-icon">
                <ul>
                <h3>FOLLOW US</h3>
                    <li><img src="@/assets/footer-facebook.png" alt=""></li>
                    <li><img src="@/assets/footer-twitter.png" alt=""></li>
                    <li><img src="@/assets/footer-youtube.png" alt=""></li>
                    <li><img src="@/assets/footer-pinterest.png" alt=""></li>
                    <li><img src="@/assets/footer-periscope.png" alt=""></li>
                </ul>
            </div>

        </div>
    </section>
</template>

<script>
export default {
    name: 'Social'
}
</script>

<style lang="scss">
@import '@/styles/variables';

.social {
    background-color: $secondary-color;
    .social-conteiner {
        height: 120px;
        display: flex;
        align-items: center;
        .social-button {
            height: 100%;
            display: flex;
            justify-content: center;
            align-items: center;
        }

        .social-icon {
            height: 100%;
            width: 100%;
            display: flex;
            ul {
                width: 100%;
                height: 100%;
                display: flex;
                justify-content: end;
                align-items: center;
                list-style: none;
                h3 {
                    color: $primary-color;
                    font-size: 24px;
                }
                li {
                    margin-left: 20px;
                }
            }
        }
    }
}



</style>