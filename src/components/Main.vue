<template>
    <main class="main">
        <section class="main-content">
            <div class="container">
                <div class="main-content-placeholder">
                    <ProductsList />
                </div>
            </div>
        </section>

        <section class="main-icon-menu">
            <div class="container">
                <ul>
                    <li>
                        <a href="#">
                            <img src="../assets/img/buy-comics-digital-comics.png" alt="">
                            <div>
                                DIGITAL COMICS
                            </div>
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <img src="../assets/img/buy-comics-merchandise.png" alt="">
                            <div>
                                DC MERCHANDISE
                            </div>
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <img src="../assets/img/buy-comics-subscriptions.png" alt="">
                            <div>
                                SUBSCRIPTION
                            </div>
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <img src="../assets/img/buy-comics-shop-locator.png" alt="">
                            <div>
                                COMIC SHOP LOCATOR
                            </div>
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <img src="../assets/img/buy-dc-power-visa.svg" alt="">
                            <div>
                                DC POWER VISA
                            </div>
                        </a>
                    </li>
                </ul>
            </div>
        </section>
    </main>
</template>

<script>
import ProductsList from "./ProductsList.vue";

export default {
    name: "Main",
    components: {
        ProductsList
    }
}
</script>

<style lang="scss" scoped>

    @import '../style/general.scss';
    @import '../style/variables.scss';

    .main {
        &-content {
            background-color: $content_back_color;

            &-placeholder {
                color: #fff;
                font-size: 25px;
                padding: 100px 0;
            }
        }

        &-icon-menu {
            background-color: lighten($logo_primary_color, 5%);
            color: #fff;
            font-size: 11px;

            ul {
                display: flex;
                justify-content: space-around;
                padding: 50px 0;
            }
            a {
                display: flex;
                align-items: center;
            }
            img {
                height: 50px;
                max-width: 50px;
                margin-right: 10px;
            }
        }
    }
</style>