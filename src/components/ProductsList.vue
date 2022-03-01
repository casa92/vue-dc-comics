<template>
    <section>
        <div class="products-wrapper">
            <ProductCard v-for="(comic, index) in comics" :key="index" :productObject="comic" />
        </div>
    </section>
</template>

<script>
import ProductCard from "./ProductCard.vue";
import comicsJson from '../assets/dc-comics.json';

export default {
    name: 'ProductsList',
    components: {
        ProductCard
    },
    data: function() {
        return {
            comics: comicsJson
        };
    }
}
</script>

<style lang="scss" scoped>
    @import '../style/general.scss';
    @import '../style/variables.scss';

    .products-wrapper {
        display: flex;
        flex-wrap: wrap;
        justify-content: space-evenly;

    }
</style>