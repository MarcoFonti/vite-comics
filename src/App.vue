<!-- JS -->
<script>

// ! IMPORTO APPHEADER
import AppHeader from './components/AppHeader.vue';
// ! IMPORTO APPMAIN
import AppMain from './components/AppMain.vue';

export default{
  name: 'MyApp',
  components: { AppHeader, AppMain } 
};
</script>

<!-- HTML -->
<template>
  <!-- HEADER -->
  <AppHeader/>
  <!-- MAIN -->
  <AppMain/>
</template>

<!-- CSS -->
<style>

</style>