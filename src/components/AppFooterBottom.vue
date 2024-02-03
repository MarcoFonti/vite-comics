<!-- JS -->
<script>

export default{
    name: 'AppFooterBottom',
    data: () => ({
        // DATI ICONE
        arrayIcon: 
        [
            {
                image:'footer-facebook.png',
                url:'#',
            },
            {
                image:'footer-twitter.png',
                url:'#',
            },
            {
                image:'footer-pinterest.png',
                url:'#',
            },
            {
                image:'footer-youtube.png',
                url:'#',
            },
            {
                image:'footer-periscope.png',
                url:'#',
            },
        ]
    }),
    
    methods: {

    // FUNZIONE URL ICONE
    createIcon(icon){
        const url = new URL(`../assets/assets-vue-dc-comics-1/img/${icon}`, import.meta.url);
        console.log(url);
        return url.href
    },
}
};

</script>

<!-- HTML -->
<template>
    <!-- FOOTER BOTTOM -->
    <footer id="recipe-footer-bottom">
        <div class="container-follow">
            <a class="sing-up" href="#">sing-up now!</a>
            <nav class="recipe-icon">
                <a class="follow" href="#">follow us</a>
                <!-- ICONE -->
                <ul><li v-for="(icon, i) in arrayIcon" :key="icon[i]"><a :href="icon.url"><img :src="createIcon(icon.image)" alt=""></a></li></ul>
            </nav>
        </div>
    </footer>
</template>

<!-- CSS -->
<style scoped>

/* RECIPIENTE BOTTOM FOOTER */
#recipe-footer-bottom {
    display: flex;
    justify-content: center;
    background-color: #303030;
    padding: 30px 0px;
}

/* CONTENITORE FOLLOW */
.container-follow {
    display: flex;
    align-items: center;
    justify-content: space-between;
    width: 1100px;
    margin: 0 auto;
}

/* LINK SING-UP */
.sing-up{
    color: #ffffff;
    border: 1px solid #0282F9;
    padding: 10px 20px;
}

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