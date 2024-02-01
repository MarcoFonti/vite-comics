<!-- JS -->
<script>

export default{
    name: 'AppFooterTop',
    data: () => ({
        // DATI DC COMICS
        arrayDcComics: 
        [
            {
                text:'Characters',
                url: '#',
            },
            {
                text:'Comics',
                url: '#',
            },
            {
                text:'Movies',
                url: '#',
            },
            {
                text:'TV',
                url: '#',
            },
            {
                text:'Games',
                url: '#',
            },
            {
                text:'Videos',
                url: '#',
            },
            {
                text:'News',
                url: '#',
            },
        ],

        // DATI SHOP
        arrayShop: 
        [
            {
                text:'Shop DC',
                url: '#',
            },
            {
                text:'Shop DC Collectibles',
                url: '#',
            },
        ],

        // DATI DC 
        arrayDc: 
        [
            {
                text:'Terms Of Use',
                url: '#',
            },
            {
                text:'Privacy policy (New)',
                url: '#',
            },
            {
                text:'Ad Choices',
                url: '#',
            },
            {
                text:'Advertising',
                url: '#',
            },
            {
                text:'Jobs',
                url: '#',
            },
            {
                text:'Subscriptions',
                url: '#',
            },
            {
                text:'Talent WorkShops',
                url: '#',
            },
            {
                text:'CPSC Cerrtificates',
                url: '#',
            },
            {
                text:'Ratings',
                url: '#',
            },
            {
                text:'Shop Help',
                url: '#',
            },
            {
                text:'Contact Us',
                url: '#',
            },
        ],

        // DATI DC SITES
        arraySites: 
        [
            {
                text:'DC',
                url: '#',
            },
            {
                text:'MAD magazine',
                url: '#',
            },
            {
                text:'DC Kids',
                url: '#',
            },
            {
                text:'DC Universe',
                url: '#',
            },
            {
                text:'DC Power Visa',
                url: '#',
            },
        ]
    }),
   
};

</script>

<!-- HTML -->
<template>
    <!-- FOOTER -->
    <footer id="recipe-footer-top">
        <!-- RECIPE NAV FOOTER -->
        <nav class="footer-row">
            <!-- RECIPE COMICS&SHOP -->
            <div class="recipe-comics-shop">
                <div class="container-comics">
                    <h4>dc comics</h4>
                    <ul><li v-for="(dcComics, i) in arrayDcComics" :key="dcComics[i]"><a :href="dcComics.url">{{ dcComics.text }}</a></li></ul>
                </div>
                <div class="container-shop">
                    <h4>shop</h4>
                    <ul><li v-for="(shop, i) in arrayShop" :key="shop[i]"><a :href="shop.url">{{ shop.text }}</a></li></ul>
                </div>
            </div>
            <!-- RECIPE DC -->
            <div class="recipe-dc">
                <h4>dc</h4>
                <ul><li v-for="(dc, i) in arrayDc" :key="dc[i]"><a :href="dc.url">{{ dc.text }}</a></li></ul>
            </div>
            <!-- RECIPE SITES -->
            <div class="recipe-sites">
                <h4>sites</h4>
                <ul><li v-for="(sites, i) in arraySites" :key="sites[i]"><a :href="sites.url">{{ sites.text }}</a></li></ul>
            </div>
        </nav>
        <!-- RECIPE IMMAGINE DC -->
        <figcaption>
            <img src="@/assets/assets-vue-dc-comics-1/img/dc-logo-bg.png" alt="Logo DC">
        </figcaption>
    </footer>

</template>

<!-- CSS -->
<style scoped>

/* RECIPE FOOTER */
#recipe-footer-top {
    background-image: url(@/assets/assets-vue-dc-comics-1/img/footer-bg.jpg);
    padding: 30px 0px;
    display: flex;
    position: relative;
}

/* IMMAGINE DC */
#recipe-footer-top img {
    width: 30%;
    height: 100%;
    position: absolute;
    top: 0;
    right: 0;
}

/* RECIPE NAV FOOTER */
.footer-row{
    display: flex;
    width: 1100px;
    margin: 0 auto;
    gap: 30px;
}

/* TITOLO LINK */
h4 {
    text-transform: uppercase;
    color: #FFFFFF;
}

/* LISTE */
ul {
    list-style: none;
    padding: 0px;
}

/* LINK */
li a {
    text-decoration: none;
    color: #797979;
}

</style>