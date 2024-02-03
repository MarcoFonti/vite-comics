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
    ],

    // DATI FILM DC
    arrayDvd: 
    [
        {
            thumb:
            'https://imgs.search.brave.com/aUNyvZBXUulb963JH7KnQm9AMr8bcBoLsiHREOqayIU/rs:fit:612:612:1/g:ce/aHR0cHM6Ly9pNS53/YWxtYXJ0aW1hZ2Vz/LmNvbS9hc3IvOWZm/ZWYzMDMtMGZhYy00/OGRkLTg3ODctYzUy/NTk0MDk2ODAwXzEu/MTc1ZDk1Mjg2NzY0/OGEwOTczMTY2NGMy/MTE1NjNlYWIuanBl/Zz9vZG5XaWR0aD02/MTImb2RuSGVpZ2h0/PTYxMiZvZG5CZz1m/ZmZmZmY',
            price: '$19.99',
            series: 'Action Comics',
            type: 'comic book',
        },
        {
            thumb:
            'https://imgs.search.brave.com/OU2E3_3vA7flyv-SJ3TcFW1d99KDlp5ZfmW9ylLLFDo/rs:fit:1012:1200:1/g:ce/aHR0cHM6Ly9pMC53/cC5jb20vd3d3LnN1/cGVycG91dm9pci5j/b20vd3AtY29udGVu/dC91cGxvYWRzLzIw/MjAvMDcvQW1lcmlj/YW4tVmFtcGlyZS0x/OTc2LTAxLWNvdi1B/bGJ1cXVlcnF1ZS0y/MDIwLmpwZz9yZXNp/emU9MTAxMiUyQzE1/NTYmc3NsPTE',
            price: '$3.99',
            series: 'American Vampire 1976',
            type: 'comic book',
        },
        {
            thumb:
            'https://imgs.search.brave.com/gAZQuZyt6WjcUWF6aXCIBaiJqtOJAK-X4nxS9Vbvwno/rs:fit:1200:1200:1/g:ce/aHR0cHM6Ly9jZG4y/LnBlbmd1aW4uY29t/LmF1L2NvdmVycy9v/cmlnaW5hbC85Nzgx/NDAxMjc1NDI2Lmpw/Zw',
            price: '$16.99',
            series: 'Aquaman',
            type: 'graphic novel',
        },
        {
            thumb:
            'https://imgs.search.brave.com/YET9wY29Aa29TyHqlbieS9qsz3HWyNYQx-WkRqdBRX4/rs:fit:640:984:1/g:ce/aHR0cDovL2dldHlv/dXJjb21pY29uLmNv/LnVrL3dwLWNvbnRl/bnQvdXBsb2Fkcy8y/MDE2LzA4L2JhdGdp/cmwtcmViaXJ0aC0x/LWNvdmVyLmpwZw',
            price: '$2.99',
            series: 'Batgirl',
            type: 'comic book',
        },
        {
            thumb:
            'https://imgs.search.brave.com/jgxYlrx442aozemzjqdmCsd9DkIkRollJp1T8sG8TfE/rs:fit:720:1106:1/g:ce/aHR0cHM6Ly9veXN0/ZXIuaWduaW1ncy5j/b20vd29yZHByZXNz/L3N0Zy5pZ24uY29t/LzIwMTgvMTAvU1RM/MDk3MDk1LTcyMHgx/MTA2LmpwZw',
            price: '$3.99',
            series: 'Batman',
            type: 'comic book',
        },
        {
            thumb:
            'https://imgs.search.brave.com/jgxYlrx442aozemzjqdmCsd9DkIkRollJp1T8sG8TfE/rs:fit:720:1106:1/g:ce/aHR0cHM6Ly9veXN0/ZXIuaWduaW1ncy5j/b20vd29yZHByZXNz/L3N0Zy5pZ24uY29t/LzIwMTgvMTAvU1RM/MDk3MDk1LTcyMHgx/MTA2LmpwZw',
            price: '$2.99',
            series: 'Batman Beyond',
            type: 'comic book',
        },
        {
            thumb:
            'https://imgs.search.brave.com/cSaB3m-tghN3_Cllp9IOlUPEPsyShCnl8gijRyPFdrg/rs:fit:791:1200:1/g:ce/aHR0cHM6Ly8xNDk0/NTUxNTIudjIucHJl/c3NhYmxlY2RuLmNv/bS93cC1jb250ZW50/L3VwbG9hZHMvMjAx/OS8wOC9CTVNNX0N2/MV9CQVQuanBn',
            price: '$3.99',
            series: 'Batman/Superman',
            type: 'comic book',
        },
        {
            thumb:
            'https://imgs.search.brave.com/jfaQd--WUx7RG8MiQ-VyCOqLUJW19ojBnjkNOG81rL4/rs:fit:666:1024:1/g:ce/aHR0cHM6Ly90aGVn/d3cuY29tL3dwLWNv/bnRlbnQvdXBsb2Fk/cy8yMDIwLzA5L0Jh/dG1hbi1TdXBlcm1h/bi1Bbm51YWwtQ3Yx/LTY2NngxMDI0Lmpw/Zw',
            price: '$4.99',
            series: 'Batman/Superman Annual',
            type: 'comic book',
        },
        {
            thumb:
            'https://imgs.search.brave.com/kSLCPBIeE9s218LRC4cIyrHOYmxrSS2Wt7LvNNfED2I/rs:fit:455:700:1/g:ce/aHR0cHM6Ly9jb21p/Y2Jvb2tyZWFsbS5j/b20vY292ZXItc2Nh/bi81ZmFmMTFjYTk1/NGQ1MGVjZDA1ZmU3/M2U1NjBiNWQyOC94/bC8tLWlzc3VlLTEu/anBn',
            price: '$5.99',
            series: 'Batman: The Joker War Zone',
            type: 'comic book',
        },
        {
            thumb:
            'https://imgs.search.brave.com/a6fAPUra4t94xMJFlYv6X7Lwm4z_qPmslx7Hiqafbok/rs:fit:600:923:1/g:ce/aHR0cHM6Ly9jZG4u/ZmxpY2tlcmluZ215/dGguY29tL3dwLWNv/bnRlbnQvdXBsb2Fk/cy8yMDIwLzA4L0Jh/dG1hbi1UaHJlZS1K/b2tlcnMtMS02MDB4/OTIzLTEuanBn',
            price: '$6.99',
            series: 'Batman: Three Jokers',
            type: 'comic book',
        },
        {
            thumb:
            'https://imgs.search.brave.com/qMxyCwK99aguaETp4ioxXLrpxwNg2JNBN3Oq7LGAgzM/rs:fit:780:1200:1/g:ce/aHR0cHM6Ly9jZG4u/ZmxpY2tlcmluZ215/dGguY29tL3dwLWNv/bnRlbnQvdXBsb2Fk/cy8yMDIwLzEwL0Jh/dG1hbi1XaGl0ZS1L/bmlnaHQtUHJlc2Vu/dHMtSGFybGV5LVF1/aW5uLTEtMS5qcGc',
            price: '$4.99',
            series: 'Batman: White Knight Presents: Harley Quinn',
            type: 'comic book',
        },
        {
            thumb:
            'https://imgs.search.brave.com/bf_FlGnymAgmvweY8YiLAcyy600JdSMl_jHpdR3t5ro/rs:fit:612:612:1/g:ce/aHR0cHM6Ly9pNS53/YWxtYXJ0aW1hZ2Vz/LmNvbS9hc3IvNTA5/M2IxOTEtZTkzZS00/NTJjLThhYTQtYTEw/ZDY0ZTcxN2E5LjA5/N2UwZWM5NDgzYzky/OGExMjY4Nzk1Nzk2/NTliZWNjLmpwZWc_/b2RuV2lkdGg9NjEy/Jm9kbkhlaWdodD02/MTImb2RuQmc9ZmZm/ZmZm',
            price: '$16.99',
            series: 'Catwoman',
            type: 'graphic novel',
        },

    ]

    }),

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
    <!-- MAIN -->
    <main>
        <section id="recipe-jumbotrom">
            <div>
                <div class="reicpe-series">current series</div>
            </div>
        </section>
        <!-- SEZIONE CONTENUTO  -->
        <section id="recipe-content">
            <div class="container-films">
                <div class="recipe-films" v-for="(films, i) in arrayDvd" :key="i">
                    <img :src="films.thumb" alt="">
                    <div class="text-films">{{ films.series }}</div>
                </div>
            </div>
            <button class="button-films">load more</button>
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
    min-height: 200px;
    background-color: #1C1C1C;
    color: #ffffff;
    display: flex;
    justify-content: center;
    align-items: center;
    padding: 40px 0px;
    flex-direction: column;
}

.container-films {
    display: flex;
    flex-wrap: wrap;
    width: 1100px;
}

.recipe-films {
    width: calc(100% / 6);
    margin: 0 auto;
}

.recipe-films img {
    width: 150px;
    height: 150px;
    margin-top: 10px;
}

.text-films {
    text-transform: uppercase;
    font-size: 12px;
}

.button-films {
    background-color:#0282F9;
    border: 1px solid #1C1C1C;
    color: #ffffff;
    padding: 10px 40px;
    text-transform: uppercase;
    margin-top: 60px;
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

#recipe-jumbotrom img {
    width: 100%;
    height: 350px;
}

#recipe-jumbotrom {
    position: relative;
    background-image: url(@/assets/assets-vue-dc-comics-1/img/jumbotron.jpg);
    min-height: 350px;
    background-size: cover;
}

.reicpe-series{
    position:absolute;
    bottom: -5%;
    left: 20%;
    text-transform: uppercase;
    color: #ffffff;
    font-weight: 600;
    background-color: #0282F9;
    padding: 10px 20px;

}

</style>