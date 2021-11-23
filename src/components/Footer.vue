<template>
    <footer class="full-width">
        <div class="footer conteiner px-15">
            <div class="footer-nav">
                <div class="footer-nav-item">
                    <h3>DC COMICS</h3>
                    <ul>
                        <li>Character</li>
                        <li>Comics</li>
                        <li>Movies</li>
                        <li>Tv</li>
                        <li>Games</li>
                        <li>Collectibles</li>
                        <li>Videos</li>
                        <li>Fans</li>
                        <li>News</li>
                        <li>Shop</li>
                    </ul>
                    <h3>SHOP</h3>
                    <ul>
                        <li>Shop DC</li>
                        <li>Shop DC Collectibles</li>
                    </ul>
                </div>
                <div class="footer-nav-item">
                    <h3>DC</h3>
                    <ul>
                        <li>Terms of Use</li>
                        <li>Privacy policy (New)</li>
                        <li>Ad Choices</li>
                        <li>Advertising</li>
                        <li>Jobs</li>
                        <li>Subscriptions</li>
                        <li>Talent Workshop</li>
                        <li>CPSC Certificates</li>
                        <li>Ratings</li>
                        <li>Shop Help</li>
                        <li>Contact Us</li>
                    </ul>
                </div>
                <div class="footer-nav-item">
                    <h3>SITES</h3>
                    <ul>
                        <li>DC</li>
                        <li>MAD Magazine</li>
                        <li>DC Kids</li>
                        <li>DC universe</li>
                        <li>DC Power Visa</li>    
                    </ul>
                </div>
                


            </div>

            <div class="footer-logo">
                <img src="@/assets/dc-logo-bg.png" alt="">
            </div>


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
    background-image: url(../assets/footer-bg.jpg);
    background-repeat: no-repeat;
    background-size: cover; 
    overflow: hidden;
    .footer {
        display: flex;
        height: 400px;

        .footer-nav {
            width: 35%;
            display: flex;
            .footer-nav-item {
                height: 100%;
                width: 100%;
                h3 {
                    color: white;
                    padding: 30px 0px 5px 0;;
                }
                ul {
                    list-style: none;
                    li {
                        color: white;
                        font-family: 'Arial', sans-serif;
                        font-weight: 200;
                        font-size: 12px;
                        color: #aaa;
                        line-height: 20px;
                    }
                }
            }
        }

        .footer-logo {
            width: 70%;
            display: flex;
            justify-content: end;
            align-items: center;
            img {
                height: 140%;
                object-fit: cover;
            }
        }
    }
}


</style>