<script>
export default{
    name: `AppFooter`,
}
</script>

<template>
    <footer>
        <section class="info-section">
            <ul>
                <li>
                    <a href="#"><img src="../assets/img/buy-comics-digital-comics.png" alt="DIGITAL COMICS">DIGITAL COMICS</a>
                </li>
                <li>
                    <a href="#"><img src="../assets/img/buy-comics-merchandise.png" alt="DIGITAL COMICS">DC MERCHANDISE</a>  
                </li>
                <li>
                    <a href="#"><img src="../assets/img/buy-comics-subscriptions.png" alt="DIGITAL COMICS">SUBSCRIPTION</a>
                </li>
                <li>
                    <a href="#"><img src="../assets/img/buy-comics-shop-locator.png" alt="">COMIC SHOP LOCATOR</a>
                </li>
                <li>
                    <a href="#"><img src="../assets/img/buy-dc-power-visa.svg" alt="DIGITAL COMICS">DC POWER VISA</a>
                </li>
                
            </ul>
        </section>
        <section class="list-section">
            <div>
                <ul>
                    <li>
                        <h3>DC COMICS</h3>
                    </li>
                    <li>
                        <a href="#">Characters</a>
                    </li>
                    <li>
                        <a href="#">Comics</a>
                    </li>
                    <li>
                        <a href="#">Movies</a>
                    </li>
                    <li>
                        <a href="#">TV</a>
                    </li>
                    <li>
                        <a href="#">Games</a>
                    </li>
                    <li>
                        <a href="#">Videos</a>
                    </li>
                    <li>
                        <a href="#">News</a>
                    </li>
                    <li>
                        <h3>SHOP</h3>
                    </li>
                    <li>
                        <a href="#">Shop DC</a>
                    </li>
                    <li>
                        <a href="#">Shop DC Collectibles</a>
                    </li>
                </ul>

                <ul>
                    <li>
                        <h3>DC</h3>
                    </li>
                    <li>
                        <a href="#">Terme of the use</a>
                    </li>
                    <li>
                        <a href="#">Privacy policy(New)</a>
                    </li>
                    <li>
                        <a href="#">Ad Choices</a>
                    </li>
                    <li>
                        <a href="#">Advertising</a>
                    </li>
                    <li>
                        <a href="#">Jobs</a>
                    </li>
                    <li>
                        <a href="#">Subscriptions</a>
                    </li>
                    <li>
                        <a href="#">Talent Worksshops</a>
                    </li>
                    <li>
                        <a href="#">CPSC Certificates</a>
                    </li>
                    <li>
                        <a href="#">Ratings</a>
                    </li>
                    <li>
                        <a href="#">Shop Help</a>
                    </li>
                    <li>
                        <a href="#">Contact Us</a>
                    </li>
                </ul>
                    
                <ul>
                    <li>
                        <h3>SITES</h3>
                    </li>
                    <li>
                        <a href="#">DC</a>
                    </li>
                    <li>
                        <a href="#">MAD Magazine</a>
                    </li>
                    <li>
                        <a href="#">DC Kids</a>
                    </li>
                    <li>
                        <a href="#">DC Universe</a>
                    </li>
                    <li>
                        <a href="#">DC Power Visa</a>
                    </li>
                </ul>
                <div class="img-container">
                    <img src="../assets/img/dc-logo-bg.png" alt="">
                </div>
            </div>   
        </section>
        <section class="sign-up-section">
            <div class="container-icon">
                <button>
                    SIGN-UP NOW
                </button>

                <div class="icon">
                    <span>FOLLOW US</span>
                    <img src="../assets/img/footer-facebook.png" alt="Facebook">
                    <img src="../assets/img/footer-twitter.png" alt="Twitter">
                    <img src="../assets/img/footer-youtube.png" alt="Youtube">
                    <img src="../assets/img/footer-pinterest.png" alt="Pinterest">
                    <img src="../assets/img/footer-periscope.png" alt="Periscope">
                </div>
            </div>
            
        </section>
    </footer>
</template>

<style lang="scss" scoped>
@use "../styles/partials/mixins" as *;
@use "../styles/partials/variables" as *;


    .info-section{
        background: $colorprimary;
        @include centerFlex();
        height: 150px;
        position: relative;
        z-index: 10;

        ul{
            @include centerFlex();
            justify-content: space-between;
            gap: 20px;
            list-style-type: none;
            width: 60%;

            li img{
                width: 50px;
                vertical-align: middle;
                margin-right: 20px;
            }

            li a{
                color: #fff;
                font-size: 15px;
            }

            
        }
    }

    .list-section{
        background-image: url(../assets/img/footer-bg.jpg);
        background-size: cover;
        background-repeat: no-repeat;
        padding-bottom: 40px;

        div{
            width: 70%;
            margin: 0 auto;
            display: flex;
            gap: 20px;
            padding-top: 20px;

            .img-container{
                position: relative;

                img{
                    width: 50%;
                    position: absolute;
                    z-index: 0;
                    top: -80px;
                    right: 20px;
                }
            }

            ul{
                list-style-type: none;
                line-height: 15px;
                margin-right: 20px;

                h3{
                    margin: 20px 0;
                    font-size: 15px;
                }

                a{
                    font-size: 12px;
                    color: #494d4f;
                }
            }
        }
    }

    .sign-up-section{
        background-color: #303030;
        @include centerFlex();
        justify-content: space-between;
        height: 100px;
        position: relative;
        z-index: 10;

        .container-icon{
            @include centerFlex();
            justify-content: space-between;
            width: 70%;
            margin: 0 auto;
            

            button{
            border: 2px solid $colorprimary;
            padding: 10px;
            cursor: pointer;
            background-color: #303030;
            color: #fff;
            }
        }

        .icon{
            @include centerFlex();

            span{
                color: $colorprimary;
            }

            img{
                margin-left: 10px;
            }
        }
    }
</style>