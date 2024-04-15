<!-- JS -->
<script>


/* ESPORTAZIONE */
export default {


    /* NOME PAGINA */
    name: 'AppFooterTopComics',


    /* PROPS CHE RICEVE UN ARRAY (DA APPFOOTERTOP) */
    props: {
        Comics: Array
    }

};

</script>

<!-- HTML -->
<template>

    <div class="container-comics">
        <h4>dc comics</h4>
        <ul>
            <!-- CICLO FOR PER RECUPERARE OGNI SINGOLO ELEMENTO E INDICE  -->
            <li v-for="(dcComics, i) in Comics" :key="i"><a :href="dcComics.url">{{ dcComics.text }}</a></li>
        </ul>
    </div>

</template>


<!-- CSS -->
<style scoped lang="scss">
/* UTILIZZO SASS */
@use '../assets/assets-vue-dc-comics-1/scss/style.scss'
</style>