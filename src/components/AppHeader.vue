<script >
export default {
  name: 'AppHeader',
  data() {
      return {
         navLinks: ['CHARACTERS', 'COMICS', 'MOVIES', 'TV', 'GAMES', 'COLLECTIBLES', 'VIDEO', 'FANS', 'NEWS', 'SHOP' ],
      }
    }
}
</script>

<template>
    <header>
       <div class="container">
            <div class="logo">
                <img src="../assets/dc-logo.png" alt="dcLogo">
            </div>
            <nav>
                <ul>
                    <li v-for="link in navLinks"><a href="#">{{link}}</a></li>
                </ul>
            </nav>
        </div> 
    </header>    
</template>

<style scoped lang="scss">
    header {
        padding: 10px;
    }
    .container {
        display: flex;
        justify-content: space-between;
        align-items: center;
            img {
                width: 50px;
            }
    }
    ul {
        display: flex;

        li {
            list-style: none;
            margin: 0 20px;
            color: var(--secondary-color);
            font-weight: bold;
            font-size: 10px;
            &:nth-child(2){
                color: var(--primary-color)
            }

            a {
                text-decoration: none;
                color:inherit;
            }
        }
    }
</style>
