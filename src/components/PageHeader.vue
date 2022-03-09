<template>
    <div class="container">
        <header class="main_header">
            <figure class="logo">
                <img src="../assets/img/dc-logo.png" alt="">
            </figure>
            <div class="navbar">
                <ul class="navbar__list">
                    <li v-for="(link,i) in links" :key="i" class="navbar__item">
                        <a href="link.href">{{link.text}}</a>
                    </li>
                    <!-- <li class="navbar__item">
                        <a href="#">Comics</a>
                    </li>
                    <li class="navbar__item">
                        <a href="#">Movies</a>
                    </li>
                    <li class="navbar__item">
                        <a href="#">TV</a>
                    </li>
                    <li class="navbar__item">
                        <a href="#">Games</a>
                    </li>
                    <li class="navbar__item">
                        <a href="#">Collectibles</a>
                    </li>
                    <li class="navbar__item">
                        <a href="#">Videos</a>
                    </li>
                    <li class="navbar__item">
                        <a href="#">Fans</a>
                    </li>
                    <li class="navbar__item">
                        <a href="#">News</a>
                    </li>
                    <li class="navbar__item">
                        <a href="#">Shop</a>
                    </li> -->
                </ul>
            </div>
        </header>
    </div>
</template>

<script>
    export default {
        name: 'PageHeader',
        data() {
            return{
                links: [
                    {
                        text: 'Characters',
                        href: '#',
                    },
                    {
                        text: 'Comics',
                        href: '#',
                    },
                    {
                        text: 'Movies',
                        href: '#',
                    },
                    {
                        text: 'Tv',
                        href: '#',
                    },
                    {
                        text: 'Games',
                        href: '#',
                    },
                    {
                        text: 'Collectibles',
                        href: '#',
                    },
                    {
                        text: 'Videos',
                        href: '#',
                    },
                    {
                        text: 'Fans',
                        href: '#',
                    },
                    {
                        text: 'News',
                        href: '#',
                    },
                    {
                        text: 'Shop',
                        href: '#',
                    },
                ]
            }
        }
    }
</script>

<style lang="scss" scoped>
$blue: #0282F9;
.container{
    max-width: 1600px;
    margin: 0 auto;
    .main_header{
        display: flex;
        justify-content: space-between;
        align-items: center;
        background-color: white;
        flex-wrap: wrap;
        .logo{
        width: max-content;
        padding: 10px;
        img{
            max-width: 75px;
            display: block;
        }
        }
        .navbar{
        display: flex;
        align-items: center;
        .navbar__list{
            display: contents;
            list-style: none;
        }
        .navbar__item{
            text-transform: uppercase;
            padding: 5px 15px;
            a{
                color: currentColor;
                text-decoration: none;
                font-weight: 400;
                position: relative;
                &:active,&:hover{
                    color: $blue;
                }
                &:hover::after{
                    position: absolute;
                    display: block;
                    content: '';
                    width: 100%;
                    height: 2px;
                    background-color: $blue;
                    top: 100%;
                }
            }
        }
    }
    }
}
</style>
