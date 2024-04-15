<!-- JS -->
<script>


/* ESPORTAZIONE */
export default {


    /* NOME PAGINA */
    name: 'AppMainFilms',


    /* PROPS CHE RICEVE UN ARRAY (DA APPMAIN) */
    props: {
        Films: Array
    }

};

</script>

<!-- HTML -->
<template>

    <!-- SEZIONE CONTENUTO  -->
    <section id="recipe-content">
        <div class="container-films">
            <!-- CICLO SULL'ARRAY E RECUPERO OGNI SINGOLO ELEMENTO E INDICE -->
            <div class="recipe-films" v-for="(films, i) in Films" :key="i">
                <img :src="films.thumb" alt="">
                <div class="text-films">{{ films.series }}</div>
            </div>
        </div>
        <button class="button-films">load more</button>
    </section>

</template>


<!-- CSS -->
<style scoped lang="scss">
/* SEZIONE CONTENUTO */
#recipe-content {
    min-height: 200px;
    background-color: #1C1C1C;
    color: #ffffff;
    display: flex;
    justify-content: center;
    align-items: center;
    padding: 40px 0px;
    flex-direction: column;
}

/* CONTENITORE FILM */
.container-films {
    display: flex;
    flex-wrap: wrap;
    width: 1100px;
}

/* RECIPIENTE FILM */
.recipe-films {
    width: calc(100% / 6);
    margin: 0 auto;
}

/* IMMAGINI */
.recipe-films {

    img {
        width: 150px;
        height: 150px;
        margin-top: 10px;
    }

}

/* TESTO */
.text-films {
    text-transform: uppercase;
    font-size: 12px;
}

/* BOTTONE */
.button-films {
    background-color: #0282F9;
    border: 1px solid #1C1C1C;
    color: #ffffff;
    padding: 10px 40px;
    text-transform: uppercase;
    margin-top: 60px;
}
</style>