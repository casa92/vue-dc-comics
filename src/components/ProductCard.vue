<template>
    <div class="product-card">
        <div class="product-img">
            <img :src="productObject.thumb" :alt="productObject.series" >
        </div>
        <div class="product-title">{{ productObject.series }}</div>
    </div>
</template>

<script>
export default {
    name: 'ProductCard',
    props: ['productObject']
}
</script>

<style lang="scss" scoped>
    @import '../style/general.scss';
    @import '../style/variables.scss';
    
    .product-card {
        width: calc((100% / 6) - 20px);
        height: 250px;
        margin: 10px;

        .product-img {
            height: 150px;

            img {
                width: 100%;
                height: 100%;
                object-fit: cover;
                object-position: top;
            }
        }

        .product-title {
                margin-top: 10px;
                text-transform: uppercase;
                font-size: 11px;
        }
    }
</style>