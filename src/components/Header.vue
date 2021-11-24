<template>
  <header class="full-width">
      <div class="header conteiner px-15">
          <div class="logo">
              <img src="@/assets/dc-logo.png" alt="">
          </div>
          <div class="nav">
              <ul>
                  <li v-for="(link, index) in navLink" :key="`link-${index}`" ><a href="link.url">{{link.text}}</a></li>
                  
              </ul>
          </div>
      </div>
  </header>
</template>

<script>
export default {
    name: 'Header',

    data() {
        return {
            navLink: [
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
            ]
        }
    }

}
</script>

<style lang="scss">
@import '@/styles/variables';

header {
    background-color: white;
    position: fixed;
    z-index: 999;
    .header {
        height: 120px;
        display: flex;
        justify-content: start;
        align-items: center;
    }

    .logo {
        height: 70%;
    }

    .nav {
        height: 100%;
        width: 100%;
        flex-grow: 1;
        ul {
            height: 100%;
            width: 100%;
            display: flex;
            justify-content: end;
            list-style: none;
            align-items: center;

            li {
                height: 100%;
                margin: 0 20px;
                display: flex;
                justify-content: center;
                align-items: center;
                cursor: pointer;
                
                a {
                    font-family: 'Open Sans Condensed', sans-serif;
                    text-decoration: none;
                    text-transform: uppercase;
                    font-weight: 700;
                    font-size: 15px;
                    color: $secondary-color;
                }
                &:hover {
                     border-bottom: 4px solid $primary-color;
                }
                &:hover a {
                    color: $primary-color;
                }

                &:last-child {
                    margin: 0;
                }
            }
        }
    }


}
</style>