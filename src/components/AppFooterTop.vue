<!-- JS -->
<script>
// IMPORTO APPFOOTERTOPCOMICS
import AppFooterTopComics from './AppFooterTopComics.vue';
// IMPORTO APPFOOTERTOPSHOP
import AppFooterTopShop from './AppFooterTopShop.vue';
// IMPORTO APPFOOTERTOPDC
import AppFooterTopDc from './AppFooterTopDc.vue';
// IMPORTO APPFOOTERTOPSITES
import AppFooterTopSites from './AppFooterTopSites.vue';



export default{
    //NOME
    name: 'AppFooterTop',
    //COMPONENTI
    components: { AppFooterTopComics, AppFooterTopShop, AppFooterTopDc, AppFooterTopSites, AppFooterTopSites },
    // PROPS
    props: {
        AppFooterTopComics: Array,
        AppFooterTopShop: Array,
        AppFooterTopDc: Array,
        AppFooterTopSites: Array
    }

};

</script>

<!-- HTML -->
<template>
    <!-- FOOTER -->
    <footer id="recipe-footer-top">
        <!-- RECIPE NAV FOOTER -->
        <nav class="footer-row">
            <!-- RECIPE COMICS&SHOP -->
            <div class="recipe-comics-shop">
                <AppFooterTopComics :Comics="AppFooterTopComics"/>
                <AppFooterTopShop :Shops="AppFooterTopShop"/>
            </div>
            <AppFooterTopDc :TopDc="AppFooterTopDc" />
            <AppFooterTopSites :TopSites="AppFooterTopSites"/>
        </nav>
        <!-- RECIPE IMMAGINE DC -->
        <figcaption>
            <img src="@/assets/assets-vue-dc-comics-1/img/dc-logo-bg.png" alt="Logo DC">
        </figcaption>
    </footer>
</template>

<!-- CSS -->
<style scoped>

/* RECIPE FOOTER */
#recipe-footer-top {
    background-image: url(@/assets/assets-vue-dc-comics-1/img/footer-bg.jpg);
    padding: 30px 0px;
    display: flex;
    position: relative;
}

/* IMMAGINE DC */
#recipe-footer-top img {
    width: 30%;
    height: 100%;
    position: absolute;
    top: 0;
    right: 0;
}

/* RECIPE NAV FOOTER */
.footer-row {
    display: flex;
    width: 1100px;
    margin: 0 auto;
    gap: 30px;
}

</style>