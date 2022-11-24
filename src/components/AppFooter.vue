<script>
export default {
  name: 'AppFooter',
}
</script>

<template>
  <footer class="">
    <div class="main-footer">
        <div class="container">
            <div class="col-dc-comics">
                <div>
                    <h3>DC COMICS</h3>
                    <nav>
                        <ul>
                            <li><a href="#">Characters</a></li>
                            <li><a href="#">Comics</a></li>
                            <li><a href="#">Movies</a></li>
                            <li><a href="#">TV</a></li>
                            <li><a href="#">Games</a></li>
                            <li><a href="#">Videos</a></li>
                            <li><a href="#">News</a></li>
                        </ul>
                    </nav>
                </div>
                <div class="col-shop">
                <h3>SHOP</h3>
                <nav>
                    <ul>
                        <li><a href="#">Shop DC</a></li>
                        <li><a href="#">Shop DC Collectibles</a></li>
                    </ul>
                </nav>
            </div>
            </div>
            <div class="col-center">
                <h3>DC COMICS</h3>
                <nav>
                    <ul>
                        <li><a href="#">Terms Of Use</a></li>
                        <li><a href="#">Privacy policy (New)</a></li>
                        <li><a href="#">Ad Choices</a></li>
                        <li><a href="#">Advertising</a></li>
                        <li><a href="#">Jobs</a></li>
                        <li><a href="#">Subscriptions</a></li>
                        <li><a href="#">Talent Workshops</a></li>
                        <li><a href="#">CPSC Certificates</a></li>
                        <li><a href="#">Ratings</a></li>
                        <li><a href="#">Shop Help</a></li>
                        <li><a href="#">Contact Us</a></li>

                    </ul>
                </nav>
            </div>
            <div class="col-right">
                <h3>SITES</h3>
                <nav>
                    <ul>
                        <li><a href="#">DC</a></li>
                        <li><a href="#">MAD Magazine</a></li>
                        <li><a href="#">DC Kids</a></li>
                        <li><a href="#">DC Universe</a></li>
                        <li><a href="#">DC Power Visa</a></li>
                    </ul>
                </nav>
            </div>
            <div class="dc-logo-big"></div>
        </div>
        
    </div>
    
    
    <div class="footer-bottom">
        <div class="container">
            <div class="sign-up">
                <button>SIGN-UP NOW!</button>
            </div>
            <div class="follow-us">
                <h2>FOLLOW-US</h2>
                <a href="#">
                    <img src="../assets/footer-facebook.png" alt="facebook-img">
                </a>
                <a href="#">
                    <img src="../assets/footer-twitter.png" alt="twitter-img">
                </a>
                <a href="#">
                    <img src="../assets/footer-youtube.png" alt="youtube-img">
                </a>
                <a href="#">
                    <img src="../assets/footer-pinterest.png" alt="pinterest-img">
                </a>
                <a href="#">
                    <img src="../assets/footer-periscope.png" alt="periscope-img">
                </a>
            </div>
        </div>
    </div>
  </footer>
</template>

<style lang="scss" scoped>

    .main-footer{
        background-image: url('../assets/footer-bg.jpg');
        background-size: cover;
        padding-top: 35px;
        padding-bottom: 40px;
        position: relative;
        z-index: -1;

        & .container{
            display: flex;
        }

        & .col-dc-comics nav:first-of-type {
            margin-bottom: 20px;
        }

        & .col-dc-comics, & .col-center, & .col-right{
            margin-right: 35px;

            & h3{
                color: white;
            }

        }

        & nav ul{
            list-style: none;
            & li a{
                text-decoration: none;
                color: #959595;
            }
            &:hover{
                color: white;
            }
            & li{
                margin: 5px 0;
                font-size: 11px;
            }
            
        }
        & .dc-logo-big{
            background-image: url('../assets/dc-logo-bg.png');
            background-position: center;
            background-repeat: no-repeat;
            height: 368px;
            width: 570px;
            position: absolute;
            top: -45px;
            right: 200px;
        }
    }
    .footer-bottom{
        background-color: var(--third-color);
        padding: 10px 0;

            & .container{
                display: flex;
                justify-content: space-between;
                align-items: center;

                & .sign-up button{
                    color: white;
                    border: 2.5px solid var(--primary-color);
                    padding: 10px 5px;
                    background-color: var(--third-color);
                }
            }

            & .follow-us{
                display: flex;
                align-items: center;
                & h2{
                    color: var(--primary-color);
                    font-size: 15px;
                    margin: 0 10px;
                }
                & img{
                    height: 30px;
                    margin-left: 1.25rem;
                }
            }
    }
    
    
</style>