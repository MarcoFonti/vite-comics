<!-- JS -->
<script>


/* ESPORTAZIONE */
export default {


    /* NOME PAGINA */
    name: 'AppFooterTopDc',


    /* PROPS CHE RICEVE UN ARRAY (DA APPFOOTERTOP) */
    props: {
        TopDc: Array
    }

};

</script>

<!-- HTML -->
<template>

    <!-- RECIPE DC -->
    <div class="recipe-dc">
        <h4>dc</h4>
        <ul>
            <!-- CICLO FOR PER RECUPERARE OGNI SINGOLO ELEMENTO E INDICE -->
            <li v-for="(dc, i) in TopDc" :key="i"><a :href="dc.url">{{ dc.text }}</a></li>
        </ul>
    </div>

</template>


<!-- CSS -->
<style scoped lang="scss">
/* UTILIZZO SASS */
@use '../assets/assets-vue-dc-comics-1/scss/style.scss'
</style>