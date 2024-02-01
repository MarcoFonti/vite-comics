<!-- JS -->
<script>
export default{
    // NOME
    name: 'AppHeader',
    // DATI
    data: () => ({
      arrayDate: 
      [
        {
          text: 'Characters',
          url: '#',
          current: false,
        },
        {
          text: 'Comics',
          url: '#',
          current: true,
        },
        {
          text: 'Movies',
          url: '#',
          current: false,
        },
        {
          text: 'TV',
          url: '#',
          current: false,
        },
        {
          text: 'Games',
          url: '#',
          current: false,
        },
        {
          text: 'Collectibles',
          url: '#',
          current: false,
        },
        {
          text: 'Videos',
          url: '#',
          current: false,
        },
        {
          text: 'Fans',
          url: '#',
          current: false,
        },
        {
          text: 'News',
          url: '#',
          current: false,
        },
        {
          text: 'Shop',
          url: '#',
          current: false,
        },
    ]
  }), 
};
</script>

<!-- HTML -->
<template>
    <!-- HEADER -->
    <header>
        <!-- RECIPENTE LOGO -->
        <figcaption class="recipe-image">
            <img src="@/assets/assets-vue-dc-comics-1/img/dc-logo.png" alt="">
        </figcaption>
        <!-- RECIPENTE LISTA LINK -->
        <nav class="recipe-nav">
            <ul>
                <li v-for="(list, i) in arrayDate" :key="list[i]"><a :href="list.url" :class="{'active' : list.current === true}">{{ list.text }}</a></li>
            </ul>
        </nav>
    </header>
</template>

<!-- CSS -->
<style scoped>

/* HEADER */
header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 10px;
    width: 1100px;
    margin: 0 auto;
}

/* LOGO */
.recipe-image img {
    width: 60px;
}

/* LISTA */
.recipe-nav ul {
    display: flex;
    gap: 20px;
    list-style: none;
}

/* LINK */
ul a {
    text-decoration: none;
    color: #303437;
    text-transform: uppercase;
}

/* LINK SELEZIONATO */
.active {
    border-bottom: 2px solid #0282F9;
}

</style>