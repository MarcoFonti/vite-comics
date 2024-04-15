<!-- JS -->
<script>


/* ESPORTAZIONE */
export default {


    /* NOME PAGINA */
    name: 'AppFooterTopSites',


    /* PROPS CHE RICEVE UN ARRAY (DA APPFOOTERTOP) */
    props: {
        TopSites: Array
    }

};

</script>


<!-- HTML -->
<template>

    <!-- RECIPE SITES -->
    <div class="recipe-sites">
        <h4>sites</h4>
        <ul>
            <!-- CICLO FOR PER RECUPERARE OGNI SINGOLO ELEMENTO E INDICE -->
            <li v-for="(sites, i) in TopSites" :key="i"><a :href="sites.url">{{ sites.text }}</a></li>
        </ul>
    </div>

</template>


<!-- CSS -->
<style scoped lang="scss">
/* UTILIZZO SASS */
@use '@/assets/assets-vue-dc-comics-1/scss/style.scss'
</style>