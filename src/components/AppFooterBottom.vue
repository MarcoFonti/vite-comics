<!-- JS -->
<script>
// IMPORTO APPFOOTERBOTTOM
import AppFooterBottomIcon from './AppFooterBottomIcon.vue';

export default{
    // NOME
    name: 'AppFooterBottom',
    // COMPONENTI
    components: { AppFooterBottomIcon, AppFooterBottomIcon },
    // PROPS
    props: {
        AppFooterBottomIcon: Array
    },
      
}

</script>

<!-- HTML -->
<template>
    <!-- FOOTER BOTTOM -->
    <footer id="recipe-footer-bottom">
        <div class="container-follow">
            <a class="sing-up" href="#">sing-up now!</a>
            <AppFooterBottomIcon :Icons="AppFooterBottomIcon"/>
        </div>
    </footer>
</template>

<!-- CSS -->
<style scoped>

/* RECIPIENTE BOTTOM FOOTER */
#recipe-footer-bottom {
    display: flex;
    justify-content: center;
    background-color: #303030;
    padding: 30px 0px;
}

/* CONTENITORE FOLLOW */
.container-follow {
    display: flex;
    align-items: center;
    justify-content: space-between;
    width: 1100px;
    margin: 0 auto;
}

/* LINK SING-UP */
.sing-up{
    color: #ffffff;
    border: 1px solid #0282F9;
    padding: 10px 20px;
}

/* LINK */
a {
    text-transform: uppercase;
    text-decoration: none;
}

</style>