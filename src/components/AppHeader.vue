<script >
export default {
  name: 'AppHeader',
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
                    <li><a href="#">CHARACTERS</a></li>
                    <li><a href="#">COMICS</a></li>
                    <li><a href="#">MOVIES</a></li>
                    <li><a href="#">TV</a></li>
                    <li><a href="#">GAMES</a></li>
                    <li><a href="#">COLLECTIBLES</a></li>
                    <li><a href="#">VIDEOS</a></li>
                    <li><a href="#">FANS</a></li>
                    <li><a href="#">NEWS</a></li>
                    <li><a href="#">SHOP</a></li>
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
