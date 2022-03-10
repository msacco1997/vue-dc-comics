<template>
    <div class="footer">
        <div class="container">
            <div class="footer_wrapper">
                <div class="footer_list">
                    <div class="list_wrapper">
                        <ul class="footer_listwrapper">
                        <h4 class="footer_title">DC Comics</h4>
                        <li class="footer_listitem"><a href="#">Footer Item</a></li>
                        <li class="footer_listitem"><a href="#">Footer Item</a></li>
                        <li class="footer_listitem"><a href="#">Footer Item</a></li>
                        <li class="footer_listitem"><a href="#">Footer Item</a></li>
                        <li class="footer_listitem"><a href="#">Footer Item</a></li>
                        <li class="footer_listitem"><a href="#">Footer Item</a></li>
                        <li class="footer_listitem"><a href="#">Footer Item</a></li>
                        </ul>

                        <ul class="footer_listwrapper">
                        <h4 class="footer_title">Shop</h4>
                        <li class="footer_listitem"><a href="#">Footer Item</a></li>
                        <li class="footer_listitem"><a href="#">Footer Item</a></li>
                        </ul>
                    </div>

                    <div class="list_wrapper">
                        <ul class="footer_listwrapper">
                        <h4 class="footer_title">DC</h4>
                        <li class="footer_listitem"><a href="#">Footer Item</a></li>
                        <li class="footer_listitem"><a href="#">Footer Item</a></li>
                        <li class="footer_listitem"><a href="#">Footer Item</a></li>
                        <li class="footer_listitem"><a href="#">Footer Item</a></li>
                        <li class="footer_listitem"><a href="#">Footer Item</a></li>
                        <li class="footer_listitem"><a href="#">Footer Item</a></li>
                        <li class="footer_listitem"><a href="#">Footer Item</a></li>
                        <li class="footer_listitem"><a href="#">Footer Item</a></li>
                        <li class="footer_listitem"><a href="#">Footer Item</a></li>
                        <li class="footer_listitem"><a href="#">Footer Item</a></li>
                        <li class="footer_listitem"><a href="#">Footer Item</a></li>
                        </ul>
                    </div>

                    <div class="list_wrapper">
                        <ul class="footer_listwrapper">
                        <h4 class="footer_title">Sites</h4>
                        <li class="footer_listitem"><a href="#">Footer Item</a></li>
                        <li class="footer_listitem"><a href="#">Footer Item</a></li>
                        <li class="footer_listitem"><a href="#">Footer Item</a></li>
                        <li class="footer_listitem"><a href="#">Footer Item</a></li>
                        <li class="footer_listitem"><a href="#">Footer Item</a></li>
                        </ul>
                    </div>
                </div>

                <div class="footer_bgimg"></div>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'PageFooter'
    }
</script>

<style lang="scss" scoped>
    .footer{
        position: relative;
        background-image: url(../assets/img/footer-bg.jpg);
        background-size: 100%;
        background-repeat: no-repeat;
        background-position: center;
        
        .container{
            max-width: 1600px;
            margin: 0 auto;
            .footer_wrapper{
                display: flex;
                width: 100%;
                .footer_list{
                    padding: 40px 0;
                    flex-grow: 1;
                    display: flex;
                    gap: 30px;
                    .list_wrapper{
                        padding: 0 10px;
                        .footer_listwrapper{
                        list-style: none;
                        color: white;
                        width: max-content;
                        .footer_title{
                            font-size: 18px;
                            font-weight: 700;
                            padding: 10px 0;
                            text-transform: uppercase;
                        }
                        .footer_listitem{
                            color: #959595;
                            a{
                                text-decoration: none;
                                color: currentColor;
                                font-size: 14px;
                            }
                        }
                    }
                    }
                    
                    
                }
                .footer_bgimg{
                    flex-grow: 1;
                    background-image: url(../assets/img/dc-logo-bg.png);
                    background-repeat: no-repeat;
                    background-size: 75%;
                    background-position: center right;
                }
            }
            
        }
    }
</style>