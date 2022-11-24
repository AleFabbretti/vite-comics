<script>
export default {
  name: 'AppDcBar',
  data(){
    return{
        cards: [
            {
                img: 'buy-comics-digital-comics.png',
                cardName: 'DIGITAL COMICS',
            },
            {
                img: 'buy-comics-merchandise.png',
                cardName: 'DC MERCHANDISE',
            },
            {
                img: 'buy-comics-subscriptions.png',
                cardName: 'SUBSCRIPTION',
            },
            {
                img: 'buy-comics-shop-locator.png',
                cardName: 'COMIC SHOP LOCATOR',
            },
            {
                img: 'buy-dc-power-visa.svg',
                cardName: 'DC POWER VISA',
            },
        ]
    }
  }
}
</script>

<template>
    <div class="dc-bar">
        <div class="cards container">
            <div class="card" v-for="card in cards">
                <a href="#" class="card-info">
                    <img :src="`src/assets/${card.img}`" alt="digital.comics-img">
                    <p>{{card.cardName}}</p>
                </a>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
    .dc-bar{
        background-color: var(--primary-color);
        padding: 40px 0;
        & .cards{
            display: flex;
            justify-content: space-between;
            align-items: center;
            & .card:nth-child(4) img{
                width: 40px;
            }
            & .card-info{
                display: flex;
                justify-content: center;
                align-items: center;
                color: white;
                text-decoration: none;
                font-size: 15px;
    
                & img{
                    width: 40px;
                    margin-right: 8px;
                    max-height: 40px;
                    
                }
            }
        }
    }
    
</style>