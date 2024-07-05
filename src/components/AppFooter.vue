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
                    <img src="../assets/img/buy-comics-digital-comics.png" alt="DIGITAL COMICS">
                    <a href="#">DIGITAL COMICS</a>
                </li>
                <li>
                    <img src="../assets/img/buy-comics-merchandise.png" alt="DIGITAL COMICS">
                    <a href="#">DC MERCHANDISE</a>
                </li>
                <li>
                    <img src="../assets/img/buy-comics-subscriptions.png" alt="DIGITAL COMICS">
                    <a href="#">SUBSCRIPTION</a>
                </li>
                <li>
                    <img src="../assets/img/buy-comics-shop-locator.png" alt="DIGITAL COMICS">
                    <a href="#">COMIC SHOP LOCATOR</a>
                </li>
                <li>
                    <img src="../assets/img/buy-dc-power-visa.svg" alt="DIGITAL COMICS">
                    <a href="#">DC POWER VISA</a>
                </li>
                
            </ul>
                
        </section>
        <section class="list-section">

        </section>
        <section class="sign-up-section">

        </section>
    </footer>
</template>

<style lang="scss" scoped>
@use "../styles/partials/mixins" as *;
@use "../styles/partials/variables" as *;


    .info-section{
        background: $colorprimary;
        @include centerFlex();
        // DEBUG
        min-height: 150px;

        ul{
            @include centerFlex();
            justify-content: space-between;
            gap: 10px;
            list-style-type: none;

            li img{
                width: 20%;
                vertical-align: middle;
                margin-right: 20px;
            }

            
        }
    }
</style>