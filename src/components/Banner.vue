<template>
    <section class="jumbotron">
        <div class="container">
            <div class="jumbotron-title-section">
               CURRENT SERIES
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'Banner',
    props: ['imgSrc']
}
</script>

<style lang="scss" scoped>

    @import '../style/general.scss';
    @import '../style/variables.scss';

    .jumbotron {
        width: 100%;
        height: 330px;
        background-image: url("../assets/img/jumbotron.jpg");
        background-position: top;
        background-size: 100%;
        
        .container {
            height: 330px;
        }

        &-title-section {
            position: absolute;
            bottom: -20px;
            left: 0;
            color: #fff;
            font-weight: bold;
            font-size: 17px;
            padding: 10px 20px;
            background-color: lighten($logo_primary_color, 5%);
        }
    }
</style>