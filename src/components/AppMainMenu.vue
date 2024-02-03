<!-- JS -->
<script>
export default{
    //NOME
    name: 'AppMainMenu',
    //PROPS
    props: {
        Menu: Array
    },
    //METODO
    methods: {
    // FUNZIONE URL IMMAGINI
    createImage(image){
        const url = new URL(`../assets/assets-vue-dc-comics-1/img/${image}`, import.meta.url);
        console.log(url);
        return url.href
        },
    }
    
};

</script>

<!-- HTML -->
<template>
    <!-- SEZIONE CONTENUTO COMICS -->
    <section id="recipe-content-comics">
        <div class="recipe-comics" v-for="(comics, i) in Menu" :key="i">
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