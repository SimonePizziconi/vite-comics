<script>
export default{
    name: `AppHeader`,
    data (){
        return {
            links: [
                {
                    text: "Characters",
                    url: "#",
                    current: false,
                },
                {
                    text: "Comics",
                    url: "#",
                    current: true,
                },
                {
                    text: "Movies",
                    url: "#",
                    current: false,
                },
                {
                    text: "TV",
                    url: "#",
                    current: false,
                },
                {
                    text: "Games",
                    url: "#",
                    current: false,
                },
                {
                    text: "Collectibles",
                    url: "#",
                    current: false,
                },
                {
                    text: "Videos",
                    url: "#",
                    current: false,
                },
                {
                    text: "Fans",
                    url: "#",
                    current: false,
                },
                {
                    text: "News",
                    url: "#",
                    current: false,
                },
                {
                    text: "Shop",
                    url: "#",
                    current: false,
                }

            ]
        }
    }
}
</script>

<template>
    <header>
        <nav>
            <a href="#">
                <img src="../assets/img/dc-logo.png" alt="Logo">
            </a>

            <ul>
                <li v-for="(link, i) in links" :key="i">
                    <a :class="{active: link.current}" :href="link.url">{{link.text}}</a>
                </li>
            </ul>
        </nav>
    </header>
</template>

<style lang="scss" scoped>
@use "../styles/partials/mixins" as *;
@use "../styles/partials/variables" as *;

    header{
        background-color: #fff;
        height: 120px;
        @include centerFlex();

        nav{
            width: 70%;
            margin: 0 auto;
            @include centerFlex ();
            justify-content: space-between;


            ul{
                @include centerFlex ();
                list-style-type: none;
                gap: 20px;
                    
                li{
                    a{
                        @include centerFlex ();
                        height: 120px;
                        align-self: center;
                    }

                    .active{
                        border-bottom: 5px solid $colorprimary;
                        color: $colorprimary;
                    }

                    a:hover{
                        color: $colorprimary;
                        border-bottom: 5px solid $colorprimary;
                    }
                }
                    
            }
        }
    }
</style>