<!-- JS -->
<script>


/* ESPORTAZIONE */
export default {


    /* NOME PAGINA */
    name: 'AppMainMenu',



    /* PROPS CHE RICEVE UN ARRAY (DA APPMAIN) */
    props: {
        Menu: Array
    },



    /* FUNZIONI */
    methods: {


        /* CREO UNA FUNZIONE PER IL PERCORSO DELLE IMMAGINI E GLI PASSO COME ARGOMENTO OGNI SINGOLA IMMAGINE */
        createImage(image) {


            /* CREO UNA VARIBILE A CUI ASSEGNO IL MERODO URL */
            const url = new URL(`../assets/assets-vue-dc-comics-1/img/${image}`, import.meta.url);


            /* CONTROLLO LA RIPOSTA */
            console.log(url);


            /* RESTITUSCO HREF DEL URL */
            return url.href
        },
    }

};

</script>

<!-- HTML -->
<template>

    <!-- SEZIONE CONTENUTO COMICS -->
    <section id="recipe-content-comics">
        <!-- CICLO SULL'ARRAY E RECUPERO OGNI SINGOLO ELEMENTO E INDICE -->
        <div class="recipe-comics" v-for="(comics, i) in Menu" :key="i">
            <!-- UTILIZZO LA FUNZIONE CREATA E GLI PASSO COME PARAMETRO LA SINGOLA IMAGGINE -->
            <img :src="createImage(comics.image)" :alt="comics.text">
            <span>{{ comics.text }}</span>
        </div>
    </section>

</template>


<!-- CSS -->
<style scoped lang="scss">

/* SEZIONE CONTENUTO COMICS */
#recipe-content-comics {
    background-color: #0282F9;
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 25px;
    text-transform: uppercase;
    padding: 50px 0px;
}

/* RECIPIENTE COMICS */
.recipe-comics {
    display: flex;
    align-items: center;
    gap: 5px;
}

/* IMMAGINI */
.recipe-comics {

    img {
        width: 40px;
    }
}

</style>