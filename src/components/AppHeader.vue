<!-- JS -->
<script>


/* IMPORTO APPHEADERNAV */
import AppHeaderNav from './AppHeaderNav.vue';


/* ESPORTAZIONE */
export default {


    /* NOME PAGINA */
    name: 'AppHeader',


    /* COMPONENTE */
    components: { AppHeaderNav },


    /* PROPS CHE RICEVE UN ARRAY (DA APP) */
    props: {
        HeaderNav: Array
    }

};

</script>

<!-- HTML -->
<template>

    <!-- HEADER -->
    <header>
        <!-- RECIPENTE LOGO -->
        <figcaption class="recipe-image">
            <img src="@/assets/assets-vue-dc-comics-1/img/dc-logo.png" alt="Immagine Logo">
        </figcaption>
        <!-- ALLA PROPS NAV PASSO UN ARRAY -->
        <AppHeaderNav :nav="HeaderNav" />
    </header>

</template>


<!-- CSS -->
<style scoped lang="scss">
/* HEADER */
header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 10px;
    width: 1100px;
    margin: 0 auto;
}

/* LOGO */
.recipe-image {

    img {
        width: 60px;
    }

}
</style>