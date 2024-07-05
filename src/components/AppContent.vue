<script>
export default{
    name: `AppContent`,
}
</script>

<template>
    <section>
        <div class="content">
            <h1> content go here <-- </h1>
        </div>
    </section>
</template>

<style lang="scss" scoped>
    @use "../styles/partials/mixins" as *;

    section{
        background-color: #000;
        @include centerFlex();
        justify-content: flex-start;
        // DEBUG
        min-height: 100px;

        .content{
            width: 70%;
            margin: 0 auto;
        }

    }
</style>