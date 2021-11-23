<template>
  <header class="full-width">
      <div class="header conteiner px-15">
          <div class="logo">
              <img src="@/assets/dc-logo.png" alt="">
          </div>
          <div class="nav">
              <ul>
                  <li><a href="">Characters</a></li>
                  <li><a href="">Comics</a></li>
                  <li><a href="">Movies</a></li>
                  <li><a href="">Tv</a></li>
                  <li><a href="">Games</a></li>
                  <li><a href="">Collectibles</a></li>
                  <li><a href="">Videos</a></li>
                  <li><a href="">Fans</a></li>
                  <li><a href="">News</a></li>
                  <li><a href="">Shop</a></li>
              </ul>
          </div>
      </div>
  </header>
</template>

<script>
export default {
    name: 'Header',

}
</script>

<style lang="scss">
@import '@/styles/variables';

header {
    background-color: white;
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
                margin: 0 10px;
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
            }
        }
    }


}
</style>