<template>
    <div class="social">
        <div class="container">
            <div class="wrapper">
                <div class="signup_btn">
                    <input type="button" class="signup" value="SIGN-UP NOW!">
                </div>
                <div class="social_cta">
                    <h4 class="social_cta_text">Follow us</h4>
                    <ul class="social_li">
                        <li class="social_li_itm">
                            <img src="../assets/img/footer-facebook.png" alt="">
                        </li>
                        <li class="social_li_itm">
                            <img src="../assets/img/footer-twitter.png" alt="">
                        </li>
                        <li class="social_li_itm">
                            <img src="../assets/img/footer-youtube.png" alt="">
                        </li>
                        <li class="social_li_itm">
                            <img src="../assets/img/footer-pinterest.png" alt="">
                        </li>
                        <li class="social_li_itm">
                            <img src="../assets/img/footer-periscope.png" alt="">
                        </li>
                    </ul>
                </div>
            
            
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'SocialFoot',
        data(){
            return{
            }
        }
    }
</script>

<style lang="scss" scoped>
    
$grey: #303030;
$blue: #0282F9;
.social{
    background-color: $grey;
    width: 100%;
    .container{
        max-width: 1600px;
        margin: 0 auto;
        .wrapper{
            display: flex;
            align-content: center;
            .signup_btn{
                flex-grow: 1;
                padding: 20px 0;
                .signup{
                    padding: 8px 15px;
                    background-color: transparent;
                    border: 2px solid $blue;
                    color: white;
                    line-height: 22px;
                }
            }
            .social_cta{
                flex-grow: 1;
                display: flex;
                justify-content: center;
                align-items: center;
                padding: 20px 0;
                .social_cta_text{
                    color: $blue;
                    text-transform: uppercase;
                    font-size: 22px;
                    padding-right: 15px;
                }
                .social_li{
                    display: flex;
                    align-items: center;
                    list-style: none;
                    justify-content: space-between;
                    gap: 15px;
                    .social_li_itm{
                        width: max-content;
                        img{
                            width: 30px;
                            display: block;
                        }
                    }
                }
            }
        }
    }
}
</style>
