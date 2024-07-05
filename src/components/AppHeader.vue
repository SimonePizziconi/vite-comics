<script>
export default{
    name: `AppHeader`,
}
</script>

<template>
    <header>
        <nav>
            <a href="#">
                <img src="../assets/img/dc-logo.png" alt="Logo">
            </a>

            <ul>
                <li>
                    <a href="#">Home</a>
                </li>
                <li>
                    <a href="#">Home</a>
                </li>
                <li>
                    <a href="#">Home</a>
                </li>
                <li>
                    <a href="#">Home</a>
                </li>
                <li>
                    <a href="#">Home</a>
                </li>
            </ul>
        </nav>
    </header>
</template>

<style lang="scss" scoped>
@use "../styles/partials/mixins" as *;

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
            }
        }
    }
</style>