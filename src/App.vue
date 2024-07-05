<script>
  import AppHeader from './components/AppHeader.vue';
  import AppContent from './components/AppContent.vue';
  import AppFooter from './components/AppFooter.vue';

  

  export default{
    name: `App`,
    components: {
      AppHeader,
      AppContent,
      AppFooter,
    }
  }
</script>

<template>
  <AppHeader/>
  <main>
    <AppContent/>
  </main>
  <AppFooter/>
</template>

<style>

</style>
