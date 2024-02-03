<!-- JS -->
<script>
export default{
    // NOME
    name: 'AppFooterBottomIcon',
    // PROPS
    props: {
        Icons: Array
    },
    // METODO
    methods: {
        // FUNZIONE URL ICONE
        createIcon(icon){
        const url = new URL(`../assets/assets-vue-dc-comics-1/img/${icon}`, import.meta.url);
        console.log(url);
        return url.href
        }
    }
}
</script>

<!-- HTML -->
<template>
    <nav class="recipe-icon">
        <a class="follow" href="#">follow us</a>
        <!-- ICONE -->
        <ul><li v-for="(icon, i) in Icons" :key="i"><a :href="icon.url"><img :src="createIcon(icon.image)" alt=""></a></li></ul>
    </nav>
</template>

<!-- CSS -->
<style scoped>

/* LINK FOLLOW */
.follow{
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