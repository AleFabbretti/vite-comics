<script>
export default {
  name: 'AppFooter',
}
</script>

<template>
  <footer>
    <div class="top">
        <div class="container">
            <img src="../assets/buy-comics-digital-comics.png" alt="digital comics">
            <img src="../assets/buy-comics-merchandise.png" alt="merchandise">
            <img src="../assets/buy-comics-subscriptions.png" alt="subscriptions">
            <img src="../assets/buy-comics-shop-locator.png" alt="shoplocator">
            <img src="../assets/buy-dc-power-visa.svg" alt="visa">
        </div>

    </div>
    <div class="center"></div>
    <div class="under"></div>
  </footer>
</template>

<style lang="scss" scoped>
    .top{
        height: 150px;
        background-color: var(--primary-color);
            & .container{
                display: flex;
                justify-content: space-around;
                padding-top: 40px;
            }
            & .container img{
                max-width: 60px;
                max-height: 60px;
            }
    }
</style>