<!-- JS -->
<script>


/* ESPORTAZIONE */
export default {


    /* NOME PAGINA */
    name: 'AppHeaderNav',


    /* PROPS CHE RICEVE UN ARRAY (DA APPHEADER) */
    props: {
        nav: Array
    }

};

</script>

<!-- HTML -->
<template>
    <!-- RECIPENTE LISTA LINK -->
    <nav class="recipe-nav">
        <ul>
            <!-- CICLO FOR PER RECUPERARE OHNI SINGOLO ELEMENTO E INDICE, METTO LA CLASSE ACTIVE SOLO ALL'ELEMENTO CON LA CHIAVE CURRENT INDENTICO A TRUE -->
            <li v-for="(list, i) in nav" :key="i"><a :href="list.url" :class="{ 'active': list.current === true }">{{
                    list.text }}</a></li>
        </ul>
    </nav>
</template>


<!-- CSS -->
<style scoped lang="scss">
/* LISTA */
.recipe-nav {

    ul {
        display: flex;
        gap: 20px;
        list-style: none;
    }

}

/* LINK */
ul {

    a {
        text-decoration: none;
        color: #303437;
        text-transform: uppercase;
    }

}

/* LINK SELEZIONATO */
.active {
    border-bottom: 2px solid #0282F9;
}
</style>