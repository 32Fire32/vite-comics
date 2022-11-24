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
                    <li><a href="#">MOVIES</a></li>
                    <li><a href="#">Link</a></li>
                    <li><a href="#">Link</a></li>
                    <li><a href="#">Link</a></li>
                    <li><a href="#">Link</a></li>
                    <li><a href="#">Link</a></li>
                    <li><a href="#">Link</a></li>
                    <li><a href="#">Link</a></li>
                    <li><a href="#">Link</a></li>
                </ul>
            </nav>
        </div> 
    </header>    
</template>

<style scoped lang="scss">
    header {
        padding: 20px;
    }
    .container {
        display: flex;
        justify-content: space-between;
        align-items: center;
    }
    ul {
        display: flex;

        li {
            list-style: none;
            margin: 0 20px;
            color: var(--secondary-color);
            font-weight: bold;

            a {
                text-decoration: none;
                color:inherit;
            }
        }
    }
</style>
