<!-- JS -->
<script>


/* ESPORTAZIONE */
export default {


    /* NOME PAGINA */
    name: 'AppFooterTopShop',


    /* PROPS CHE RICEVE UN ARRAY (DA APPFOOTERTOP) */
    props: {
        Shops: Array
    }

};
</script>

<!-- HTML -->
<template>

    <div class="container-shop">
        <h4>shop</h4>
        <ul>
            <!-- CICLO FOR PER RECUPERARE OGNI SINGOLO ELEMENTO E INDICE -->
            <li v-for="(shop, i) in Shops" :key="i"><a :href="shop.url">{{ shop.text }}</a></li>
        </ul>
    </div>

</template>


<!-- CSS -->
<style scoped lang="scss">
/* UTILIZZO SASS */
@use '../assets/assets-vue-dc-comics-1/scss/style.scss'
</style>