<template>
    <div class="cta">
        <div class="container">
            <div class="wrapper">
                <ul class="list">
                    <li v-for="(item, i) in items" :key="i" class="list_item">
                        <figure>
                            <img v-bind:src="item.image" alt="">
                        </figure>
                        <h4 class="list_text">{{item.text}}</h4>
                    </li>
                    <!--<li class="list_item">
                        <figure>
                            <img src="../assets/img/buy-comics-merchandise.png" alt="">
                        </figure>
                        <h4 class="list_text">
                            merchandise
                        </h4>
                    </li>
                    <li class="list_item">
                        <figure>
                            <img src="../assets/img/buy-comics-subscriptions.png" alt="">
                        </figure>
                        <h4 class="list_text">
                            subscription
                        </h4>
                    </li>
                    <li class="list_item">
                        <figure>
                            <img src="../assets/img/buy-comics-shop-locator.png" alt="">
                        </figure>
                        <h4 class="list_text">
                            Comic Shop locator
                        </h4>
                    </li>
                    <li class="list_item">
                        <figure>
                            <img src="../assets/img/buy-dc-power-visa.svg" alt="">
                        </figure>
                        <h4 class="list_text">
                            DC power visa
                        </h4>
                    </li>-->
                </ul>
            </div>
        </div>
    </div>
</template>


<script>
    export default {
        name: 'CtaList',
        data(){
            return{
                items:[
                    {
                        image: require('../assets/img/buy-comics-digital-comics.png'),
                        text: 'Digital Comics',
                    },
                    {
                        image: require('../assets/img/buy-comics-merchandise.png'),
                        text: 'DC Merchandise',
                    },
                    {
                        image: require('../assets/img/buy-comics-subscriptions.png'),
                        text: 'Subscription',
                    },
                    {
                        image: require('../assets/img/buy-comics-shop-locator.png'),
                        text: 'Comic shop locator',
                    },
                    {
                        image: require('../assets/img/buy-dc-power-visa.svg'),
                        text: 'DC power visa',
                    },
                ],
            }
        }
    }
</script>




<style lang="scss" scoped>
$blue: #0282F9;
        .cta{
            width: 100%;
            background-color: $blue;
            height: 120px;
            .container{
                max-width: 1600px;
                margin: 0 auto;
                .wrapper{
                    padding: 35px 0;
                    .list{
                    list-style: none;
                    display: flex;
                    align-items: center;
                    justify-content: space-between;
                    gap: 8px;
                    padding: 0 25px;
                        .list_item{
                        display: flex;
                        align-items: center;
                        gap: 18px;
                            figure{
                                width: max-content;
                                img{
                                    height: 40px;
                                }
                            }
                            .list_text{
                                color: white;
                                font-family: 'OpenSans', sans-serif;
                                text-transform: uppercase;
                                font-weight: 300;
                                font-size: 15px;
                            }
                        }
                    }
                }
            }
    }
</style>