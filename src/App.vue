<!-- JS -->
<script>

// ! IMPORTO APPHEADER
import AppHeader from './components/AppHeader.vue';
// ! IMPORTO APPMAIN
import AppMain from './components/AppMain.vue';
// ! IMPORTO APPFOOTERTOP
import AppFooterTop from './components/AppFooterTop.vue';
// ! IMPORTO APPFOOTERBOTTOM
import AppFooterBottom from './components/AppFooterBottom.vue';


export default{
  name: 'MyApp',
  components: { AppHeader, AppMain, AppFooterTop, AppFooterBottom } 
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
  <!-- FOOTER BOOTOM -->
  <AppFooterBottom/>
</template>

<!-- CSS -->
<style>

</style>