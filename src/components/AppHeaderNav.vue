<!-- JS -->
<script>
export default{
    //NOME
    name: 'AppHeaderNav',
    //PROPS
    props: {
        nav: Array
    } 

};

</script>

<!-- HTML -->
<template>
    <!-- RECIPENTE LISTA LINK -->
    <nav class="recipe-nav">
        <ul>
            <li v-for="(list, i) in nav" :key="i"><a :href="list.url" :class="{'active' : list.current === true}">{{ list.text }}</a></li>
        </ul>
    </nav>
</template>

<!-- CSS -->
<style scoped lang="scss">

/* LISTA */
.recipe-nav{
    
    ul {
        display: flex;
        gap: 20px;
        list-style: none;
    }
    
}

/* LINK */
ul {
    
    a {
    text-decoration: none;
    color: #303437;
    text-transform: uppercase;
    }

}

/* LINK SELEZIONATO */
.active {
    border-bottom: 2px solid #0282F9;
}

</style>