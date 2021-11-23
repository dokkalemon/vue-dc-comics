<template>
    <footer class="full-width">
        <div class="footer conteiner px-15">
            <div class="footer-nav">
                <div class="footer-nav-item">
                    <h3>DC COMICS</h3>
                    <ul>
                        <li v-for="(link, index) in dcComicsLink" :key="`dcComicsLink-${index}`"><a href="link.url">{{link.text}}</a></li>
                        
                    </ul>
                    <h3>SHOP</h3>
                    <ul>
                        <li v-for="(link, index) in shopLink" :key="`shopLink-${index}`"><a href="link.url">{{link.text}}</a></li>  
                    </ul>
                </div>
                <div class="footer-nav-item">
                    <h3>DC</h3>
                    <ul>
                        <li v-for="(link, index) in dcLink" :key="`dcLink-${index}`"><a href="link.url">{{link.text}}</a></li>  
                    </ul>
                </div>
                <div class="footer-nav-item">
                    <h3>SITES</h3>
                    <ul>
                        <li v-for="(link, index) in sitesLink" :key="`dcComicsLink-${index}`"><a href="link.url">{{link.text}}</a></li>
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
    name: 'Footer',

    data() {
        return {
            dcComicsLink: [
                 {
                    text: 'Characters',
                    url: '/characters',
                    current: true
                },
                {
                    text: 'Comics',
                    url: '/comics',
                    current: true
                },
                {
                    text: 'Movies',
                    url: '/movies',
                    current: true
                },
                {
                    text: 'Tv',
                    url: '/tv',
                    current: true
                },
                {
                    text: 'Games',
                    url: '/games',
                    current: true
                },
                {
                    text: 'Collectibles',
                    url: '/collectibles',
                    current: true
                },
                {
                    text: 'Videos',
                    url: '/videos',
                    current: true
                },
                {
                    text: 'Fans',
                    url: '/fans',
                    current: true
                },
                {
                    text: 'News',
                    url: '/news',
                    current: true
                },
                {
                    text: 'Shop',
                    url: '/shop',
                    current: true
                },
            ],

            shopLink: [
                {
                    text: 'Shop DC',
                    url: '/shop-dc',
                    current: true
                },
                {
                    text: 'Shop DC Collectibles',
                    url: '/shop-dc-collectibles',
                    current: true
                }
            ],

            dcLink: [
                {
                    text: 'Terms of Use',
                    url: '/terms-of-use',
                    current: true,
                },
                {
                    text: 'Privacy policy (New)',
                    url: '/privacy-policy',
                    current: true,
                },
                {
                    text: 'Ad Choise',
                    url: '/ad-choise',
                    current: true,
                },
                {
                    text: 'Advertising',
                    url: '/advertising',
                    current: true,
                },
                {
                    text: 'Jobs',
                    url: '/jobs',
                    current: true,
                },
                {
                    text: 'Subscription',
                    url: '/subscription',
                    current: true,
                },
                {
                    text: 'Talent Workshop',
                    url: '/talent-workshop',
                    current: true,
                },
                {
                    text: 'CPSC Certificates',
                    url: '/cpsc-certificates',
                    current: true,
                },
                {
                    text: 'Ratings',
                    url: '/ratings',
                    current: true,
                },
                {
                    text: 'Shop Help',
                    url: '/shop-help',
                    current: true,
                },
                {
                    text: 'Contact Us',
                    url: '/contact-us',
                    current: true,
                },
                ],

            sitesLink: [
                {
                    text: 'DC',
                    url: '/dc',
                    current: true,
                },
                {
                    text: 'MAD Magazine',
                    url: '/mad-magazine',
                    current: true,
                },
                {
                    text: 'DC Kids',
                    url: '/dc-kids',
                    current: true,
                },
                {
                    text: 'DC universe',
                    url: '/dc-universe',
                    current: true,
                },
                {
                    text: 'DC Power Visa',
                    url: '/dc-power-visa',
                    current: true,
                },
            ]
        }
    }
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
                        font-family: 'Arial', sans-serif;
                        font-weight: 200;
                        font-size: 12px;
                        color: #aaa;
                        line-height: 20px;
                        a {
                            color: #aaa;
                            text-decoration: none;

                        }
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