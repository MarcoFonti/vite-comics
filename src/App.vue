<!-- JS -->
<script>

// ! IMPORTO APPHEADER
import AppHeader from './components/AppHeader.vue';
// ! IMPORTO APPMAIN
import AppMain from './components/AppMain.vue';
// ! IMPORTO APPFOOTERTOP
import AppFooterTop from './components/AppFooterTop.vue';

export default{
  name: 'MyApp',
  components: { AppHeader, AppMain, AppFooterTop } 
};
</script>

<!-- HTML -->
<template>
  <!-- HEADER -->
  <AppHeader/>
  <!-- MAIN -->
  <AppMain/>
    <!-- FOOTER-TOP -->
    <AppFooterTop/>
</template>

<!-- CSS -->
<style>

</style>