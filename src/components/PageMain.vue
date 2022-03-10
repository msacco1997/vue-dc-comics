<template>
    <div class="jumbotron">
        <div class="bg">

        </div>
        <div class="container">
            
            <div class="grid">
                <JumboCard v-for="(element, i) in thumbsArray" :key="i" :thumb="element.thumb" :series="element.series" />
            </div>
            <div class="load_wrapper">
                <input class="load" type="button" value="Load More">
            </div>
        </div>
    </div>
</template>

<script>
    import JumboCard from '@/components/JumboCard.vue'
    export default {
        name: 'PageMain',
        components: {
            JumboCard,
        },
        
        data(){
            return{
                text: '--> Content goes here <--',
                thumbsArray: [
                                {
                                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX",
                                    "price": "$19.99",
                                    "series": "Action Comics",
                                    "type": "comic book"
                                },
                                {
                                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01",
                                    "price": "$3.99",
                                    "series": "American Vampire 1976",
                                    "type": "comic book"
                                },
                                {
                                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb",
                                    "price": "$16.99",
                                    "series": "Aquaman",
                                    "type": "graphic novel"
                                },
                                {
                                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/06/batgirl_v5_1_5b23e1f1124941.50950783.jpg?itok=VnrJah76",
                                    "price": "$2.99",
                                    "series": "Batgirl",
                                    "type": "comic book"
                                },
                                {
                                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
                                    "price": "$3.99",
                                    "series": "Batman",
                                    "type": "comic book"
                                },
                                {
                                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
                                    "price": "$2.99",
                                    "series": "Batman Beyond",
                                    "type": "comic book"
                                },
                                {
                                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2019/08/BMSM_5d4361b7116261.74371456.jpg?itok=kEDR2OL8",
                                    "price": "$3.99",
                                    "series": "Batman/Superman",
                                    "type": "comic book"
                                },
                                {
                                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMSMANN_01_300-001_HD_5f5ff17fa1d665.74704970.jpg?itok=azz5sfGk",
                                    "price": "$4.99",
                                    "series": "Batman/Superman Annual",
                                    "type": "comic book"
                                },
                                {
                                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMTJWZ_01_300-001_HD_5f5ff2307dcb37.34652945.jpg?itok=VswVjLR8",
                                    "price": "$5.99",
                                    "series": "Batman: The Joker War Zone",
                                    "type": "comic book"
                                },
                                {
                                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/08/cover-v2_5f40314645a734.37285065.png?itok=ImNM2QBY",
                                    "price": "$6.99",
                                    "series": "Batman: Three Jokers",
                                    "type": "comic book"
                                },
                                {
                                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/10/BMWK_HQ_01_300-001_HD_5f7cb4945e13f6.89501032.jpg?itok=sVwALbUX",
                                    "price": "$4.99",
                                    "series": "Batman: White Knight Presents: Harley Quinn",
                                    "type": "comic book"
                                },
                                {
                                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2019/04/CTWv1_CC_144-001_HD_5ca5299a751963.53054221.jpg?itok=ooPaoLDq",
                                    "price": "$16.99",
                                    "series": "Catwoman",
                                    "type": "graphic novel"
                                }
                                ],
            }
        }
    }
</script>

<style lang="scss" scoped>
    $blue: #0282F9;
    $black: #1C1C1C;
    .jumbotron{
        width: 100%;
        background-color: $black;
        
        .bg{
            height: 350px;
            background-image: url(../assets/img/jumbotron.jpg);
            background-size: 100%;
            background-position: top;
            background-repeat: no-repeat;
        }
        
        
        .container{
        max-width: 1600px;
        margin: 0 auto;
        position: relative;
        
        
        &::after{
            position: absolute;
            top: -15px;
            left: -10px4;
            width: max-content;
            display: block;
            content: 'Current Series';
            text-transform: uppercase;
            background-color: $blue;
            padding: 8px 19px;
            color: white;
            font-weight: 700;
            z-index: 504;
            }
            .grid{
                padding: 40px 0;
                width: 100%;
                display: flex;
                gap: 20px;
                flex-wrap: wrap;
                justify-content: center;
            }
            .load_wrapper{
                padding-top: 25px;
                padding-left: 45%;
                padding-bottom: 15px;
                .load{
                    text-transform: uppercase;
                    color: white;
                    background-color: $blue;
                    padding: 10px 30px;
                    border: none;
                    font-weight: 700;
                }
            }
        }
    }
</style>