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
        <nav class="header__nav">
            <ul>
                <li v-for="link in menuLinks"><a href="#">{{link.linkName}}</a></li>
            </ul>
        </nav>
    </header>
  
</template>

<style lang="scss" scoped>
    .header{
        display: flex;
        justify-content: space-between;
            & img{
                max-width: 4.375rem;
                margin: .9375rem 0;
            }
            & ul{
                height: 100%;
                display: flex;
                align-items: center;
                list-style: none;
            }
        }



</style>