<!-- JS -->
<script>


/* ESPORTAZIONE */
export default {


    /* NOME PAGINA */
    name: 'AppFooterBottomIcon',


    /* PROPS CHE RICEVE UN ARRAY (DA APPFOOTERBOTTOM) */
    props: {
        Icons: Array
    },


    /* FUNZIONI */
    methods: {


        /* CREO UNA FUNZIONE PER IL PERCORSO DELLE IMMAGINI(ICONA) E GLI PASSO COME ARGOMENTO OGNI SINGOLA IMMAGINE(ICONA) */
        createIcon(icon) {


            /* CREO UNA VARIBILE A CUI ASSEGNO IL MERODO URL */
            const url = new URL(`../assets/assets-vue-dc-comics-1/img/${icon}`, import.meta.url);


            /* CONTROLLO LA RIPOSTA */
            console.log(url);


            /* RESTITUSCO HREF DEL URL */
            return url.href
        },
    }
}

</script>


<!-- HTML -->
<template>

    <nav class="recipe-icon">
        <a class="follow" href="#">follow us</a>
        <!-- ICONE -->
        <ul>
            <!-- CICLO SULL'ARRAY E RECUPERO OGNI SINGOLO ELEMENTO E INDICE -->
            <li v-for="(icon, i) in Icons" :key="i">
                <!--  UTILIZZO LA FUNZIONE CREATA E GLI PASSO COME PARAMETRO LA SINGOLA IMAGGINE -->
                <a :href="icon.url"><img :src="createIcon(icon.image)" alt=""></a>
            </li>
        </ul>
    </nav>

</template>


<!-- CSS -->
<style scoped>
/* LINK FOLLOW */
.follow {
    color: #0282F9;
    font-weight: 600;
}

/* RECIPIENTE ICONE */
.recipe-icon {
    display: flex;
    align-items: center;
}

/* LISTE ICONE */
ul {
    display: flex;
    gap: 10px;
    list-style: none;
}

/* LINK */
a {
    text-transform: uppercase;
    text-decoration: none;
}
</style>