<template>
    <footer class="footer">
        <section class="footer-top">
            <div class="container footer-top-wrapper">
                <div class="footer-top-menu">
                    
                    <div class="footer-top-menu-column">
                        <h3>DC COMICS</h3>
                        <ul>
                            <li>
                                <a href="#">Prova</a>
                            </li>
                            <li>
                                <a href="#">Prova</a>
                            </li>
                            <li>
                                <a href="#">Prova</a>
                            </li>
                            <li>
                                <a href="#">Prova</a>
                            </li>
                            <li>
                                <a href="#">Prova</a>
                            </li>
                            <li>
                                <a href="#">Prova</a>
                            </li>
                            <li>
                                <a href="#">Prova</a>
                            </li>
                        </ul>

                        <h3>SHOP</h3>
                        <ul>
                            <li>
                                <a href="#">Prova</a>
                            </li>
                            <li>
                                <a href="#">Prova</a>
                            </li>
                        </ul>
                    </div>

                    <div class="footer-top-menu-column">
                        <h3>DC</h3>
                        <ul>
                            <li>
                                <a href="#">Prova</a>
                            </li>
                            <li>
                                <a href="#">Prova</a>
                            </li>
                            <li>
                                <a href="#">Prova</a>
                            </li>
                            <li>
                                <a href="#">Prova</a>
                            </li>
                            <li>
                                <a href="#">Prova</a>
                            </li>
                            <li>
                                <a href="#">Prova</a>
                            </li>
                            <li>
                                <a href="#">Prova</a>
                            </li>
                            <li>
                                <a href="#">Prova</a>
                            </li>
                            <li>
                                <a href="#">Prova</a>
                            </li>
                            <li>
                                <a href="#">Prova</a>
                            </li>
                            <li>
                                <a href="#">Prova</a>
                            </li>
                        </ul>

                    </div>
                    
                    <div class="footer-top-menu-column">
                        <h3>SITES</h3>
                        <ul>
                            <li>
                                <a href="#">Prova</a>
                            </li>
                            <li>
                                <a href="#">Prova</a>
                            </li>
                            <li>
                                <a href="#">Prova</a>
                            </li>
                            <li>
                                <a href="#">Prova</a>
                            </li>
                            <li>
                                <a href="#">Prova</a>
                            </li>
                        </ul>
                    </div>
                </div>
                <div class="footer-top-logo">
                    <img src="../assets/img/dc-logo-bg.png" alt="">
                </div>
            </div>
        </section>

        <section class="footer-bottom">

        </section>
    </footer>
</template>

<script>
    export default {
        name: "Footer",
    }
</script>

<style lang="scss" scoped>
    @import '../style/general.scss';
    @import '../style/variables.scss';

    .footer {
        &-top {
            background-image: url('../assets/img/footer-bg.jpg');
            background-repeat: no-repeat;
            background-size: cover;
            overflow: hidden;
            
            &-wrapper {
                display: flex;
                justify-content: space-between;
            }

            &-menu {
                color: #fff;
                padding: 50px 0;
                display: flex;

                &-column {
                    margin-right: 50px;
                }

                ul {
                    margin: 15px 0;

                    li {
                        font-size: 12px;
                        line-height: 19px;
                    }
                }
            }

            &-logo {
                img {
                    position: absolute;
                    // top: 50%;
                    // bottom: 50%;
                    // transform: translate(-50%, -50%);
                    top: -25%;
                    right: 0;
                    
                }
            }
        }
    }

</style>
