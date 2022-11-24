<script>
export default {
  name: 'AppHeader',
  data() {
    return{
        menuLinks: [
                    {
                        linkName: 'CHARACTERS',
                    },
                    {
                        linkName: 'COMICS',
                    },
                    {
                        linkName: 'MOVIES',
                    },
                    {
                        linkName: 'TV',
                    },
                    {
                        linkName: 'GAMES',
                    },
                    {
                        linkName: 'COLLECTIBLES',
                    },
                    {
                        linkName: 'VIDEOS',
                    },
                    {
                        linkName: 'FANS',
                    },
                    {
                        linkName: 'NEWS',
                    },
                    {
                        linkName: 'SHOP',
                    }
                ]
    }
    
  }
}
</script>

<template>
    <header class="container">
        <div class="logo">
            <img src="../assets/dc-logo.png" alt="logo">
        </div>
        <nav class="nav">
            <ul>
                <li v-for="link in menuLinks"><a href="#">{{link.linkName}}</a></li>
            </ul>
        </nav>
    </header>
  
</template>

<style lang="scss" scoped>
    header{
        display: flex;
        justify-content: space-between;
            & .logo img{
                max-width: 70px;
                margin: 15px 0;
            }
            & .nav ul{
                height: 100%;
                display: flex;
                align-items: center;
                list-style: none;
            }
            & .nav ul li{
                margin-left: 25px;
            }
            & .nav ul li a{
                text-decoration: none;
                color: var(--secondary-color);
                font-size: 15px;
                &:hover{
                    color: var(--primary-color);
                }
            }
        }



</style>