<template>
    <header class="header">
        <div class="container header-wrapper">
            <div class="header-logo">
                <img src="../assets/img/dc-logo.png" alt="">
            </div>
            <div class="header-menu">
                <ul>
                    <li v-for="(link, index) in links" :class="{ 'active': link.current }" :key="index">
                        <a :href="link.url">
                            {{ link.linkText }}
                        </a>
                    </li>
                    <!-- <li>
                        <a href="#">CHARACTERS</a>
                    </li>
                    <li class="active">
                        <a href="#">COMICS</a>
                    </li>
                    <li>
                        <a href="#">MOVIES</a>
                    </li>
                    <li>
                        <a href="#">TV</a>
                    </li>
                    <li>
                        <a href="#">GAMES</a>
                    </li>
                    <li>
                        <a href="#">COLLECTIBLES</a>
                    </li>
                    <li>
                        <a href="#">VIDEOS</a>
                    </li>
                    <li>
                        <a href="#">FANS</a>
                    </li>
                    <li>
                        <a href="#">NEWS</a>
                    </li>
                    <li>
                        <a href="#">SHOP</a>
                    </li> -->
                </ul>
            </div>
        </div>
    </header>
</template>

<script>
export default {
    name: "Header",
    data: function() {
        return {
            links: [
                {
                    linkText: 'CHARACTERS',
                    url: '#',
                    current: false
                },
                {
                    linkText: 'COMICS',
                    url: '#',
                    current: true
                },
                {
                    linkText: 'MOVIES',
                    url: '#',
                    current: false
                },
                {
                    linkText: 'TV',
                    url: '#',
                    current: false
                },
                {
                    linkText: 'GAMES',
                    url: '#',
                    current: false
                },
                {
                    linkText: 'COLLECTIBLES',
                    url: '#',
                    current: false
                },
                {
                    linkText: 'VIDEOS',
                    url: '#',
                    current: false
                },
                {
                    linkText: 'FANS',
                    url: '#',
                    current: false
                },
                {
                    linkText: 'NEWS',
                    url: '#',
                    current: false
                },
                {
                    linkText: 'SHOP',
                    url: '#',
                    current: false
                }
            ]
        }
    }
}
</script>

<style lang="scss" scoped>

    @import '../style/variables.scss';

    .header {
        background-color: #fff;
        height: 120px;
        line-height: 120px;

        &-wrapper {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        &-logo {
            img {
                width: 80px;
                vertical-align: middle;
            }
        }
        &-menu {
            font-size: 11px;
            font-weight: bold;
        
            ul {
                display: flex;
                justify-content: space-between;

                li {
                    margin-left: 30px;
                    line-height: 115px;

                    a {
                        display: inline-block;
                        
                    }
                }

                .active {
                        color: $logo_primary_color;
                        border-bottom: 5px solid $logo_primary_color;
                }

            }
        }
    }
</style>