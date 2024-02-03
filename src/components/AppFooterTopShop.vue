<!-- JS -->
<script>
export default{
    //NOME
    name: 'AppFooterTopShop',
    //PROPS
    props: {
        Shops: Array
    }
    
};
</script>

<!-- HTML -->
<template>
    <div class="container-shop">
        <h4>shop</h4>
        <ul><li v-for="(shop, i) in Shops" :key="i"><a :href="shop.url">{{ shop.text }}</a></li></ul>
    </div>
</template>

<!-- CSS -->
<style scoped lang="scss">

/* UTILIZZO SASS */
@use '../assets/assets-vue-dc-comics-1/scss/style.scss'

</style>