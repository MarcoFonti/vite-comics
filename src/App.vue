<!-- JS -->
<script>


/* IMPORTO APPHEADER */
import AppHeader from './components/AppHeader.vue';
/* MPORTO APPMAIN */
import AppMain from './components/AppMain.vue';
/* IMPORTO APPFOOTERTOP */
import AppFooterTop from './components/AppFooterTop.vue';
/* IMPORTO APPFOOTERBOTTOM */
import AppFooterBottom from './components/AppFooterBottom.vue';
/* IMPORTO FILE INDEX.JS */
import { FooterBottomIcon, FooterTopComics, FooterTopDc, FooterTopShop, FooterTopSites, HeaderNav, MainFilms, MainMenu } from './assets/date/index';


/* ESPORTAZIONE */
export default {


  /* NOME PAGINA */
  name: 'MyApp',


  /* DATI DI BASE DA UTILIZZARE NEL TEMPLATE (UTILIZZANDO LE PROPS) */
  data: () => ({
    FooterBottomIcon,
    FooterTopComics,
    FooterTopDc,
    FooterTopShop,
    FooterTopSites,
    HeaderNav,
    MainFilms,
    MainMenu,
  }),


  /* COMPONENTI */
  components: { AppHeader, AppMain, AppFooterTop, AppFooterBottom }
};
</script>


<!-- HTML -->
<template>

  <!-- HEADER -->
  <AppHeader :HeaderNav="HeaderNav" />

  <!-- MAIN -->
  <AppMain :AppMainFilms="MainFilms" :AppMainMenu="MainMenu" />

  <!-- FOOTER-TOP -->
  <AppFooterTop :AppFooterTopComics="FooterTopComics" :AppFooterTopShop="FooterTopShop" :AppFooterTopDc="FooterTopDc"
    :AppFooterTopSites="FooterTopSites" />

  <!-- FOOTER BOOTOM -->
  <AppFooterBottom :AppFooterBottomIcon="FooterBottomIcon" />

</template>


<!-- CSS -->
<style>
/* BODY */
body {
  height: 100vh;
}
</style>