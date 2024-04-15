<!-- JS -->
<script>


/* IMPORTO APPMAINFILMS */
import AppMainFilms from './AppMainFilms.vue';
/* IMPORTO APPMAINMENU */
import AppMainMenu from './AppMainMenu.vue';


/* ESPORTAZIONE */
export default {


    /* NOME PAGINA */
    name: 'AppMain',


    /* COMPONENTI */
    components: { AppMainFilms, AppMainMenu },


    /* PROPS CHE RICEVE DUE ARRAY (DA APP) */
    props: {
        AppMainFilms: Array,
        AppMainMenu: Array
    },

};

</script>

<!-- HTML -->
<template>

    <!-- MAIN -->
    <main>
        <section id="recipe-jumbotrom">
            <div>
                <div class="reicpe-series">current series</div>
            </div>
        </section>
        <!-- ALLA PROPS FILMS PASSO UN ARRAY -->
        <AppMainFilms :Films="AppMainFilms" />
        <!-- ALLA PROPS MENU PASSO UN ARRAY -->
        <AppMainMenu :Menu="AppMainMenu" />
    </main>

</template>


<!-- CSS -->
<style scoped lang="scss">
/* IMMAGINE JUMBOTROM */
#recipe-jumbotrom {

    img {
        width: 100%;
        height: 350px;
    }

}

/* RECIPIENTE JUMBOTROM */
#recipe-jumbotrom {
    position: relative;
    background-image: url(@/assets/assets-vue-dc-comics-1/img/jumbotron.jpg);
    min-height: 350px;
    background-size: cover;
}

/* RECIPENTE CURRENT SERIES */
.reicpe-series {
    position: absolute;
    bottom: -5%;
    left: 20%;
    text-transform: uppercase;
    color: #ffffff;
    font-weight: 600;
    background-color: #0282F9;
    padding: 10px 20px;
}
</style>