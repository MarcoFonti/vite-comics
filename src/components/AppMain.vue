<!-- JS -->
<script>

export default{
  name: 'AppMain',
  data: ()=> ({
    // DATI COMICS
    arrayComics: 
    [
        {
            image: 'buy-comics-digital-comics.png',
            text: 'digital comics',
        },
        {
            image: 'buy-comics-merchandise.png',
            text: 'dc merchandise',
        },
        {
            image: 'buy-comics-subscriptions.png',
            text: 'subscription',
        },
        {
            image: 'buy-comics-shop-locator.png',
            text: 'comic shop locator',
        },
        {
            image: 'buy-dc-power-visa.svg',
            text: 'dc power visa',
        }
    ]
  }),

  methods: {

    // FUNZIONE URL IMMAGINI
    createImage(image){
        const url = new URL(`../assets/assets-vue-dc-comics-1/img/${image}`, import.meta.url);
        console.log(url);
        return url.href
    }
  }
};

</script>

<!-- HTML -->
<template>
    <!-- MAIN -->
    <main>
        <!-- SEZIONE CONTENUTO  -->
        <section id="recipe-content">
            <div>Content goes here</div>
        </section>
        <!-- SEZIONE CONTENUTO COMICS -->
        <section id="recipe-content-comics">
            <div class="recipe-comics" v-for="(comics, i) in arrayComics" :key="comics[i]">
                <img :src="createImage(comics.image)" alt="">
                <span>{{ comics.text }}</span>
            </div>
        </section>
    </main>
</template>

<!-- CSS -->
<style scoped>

/* SEZIONE CONTENUTO */
#recipe-content {
    min-height: 100px;
    background-color: #1C1C1C;
    color: #ffffff;
}

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
.recipe-comics img {
    width: 40px;
}

</style>