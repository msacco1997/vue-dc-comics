<template>
    <div >
        <div class="card">
            <figure class="thumb_wrapper">
                <img :src="thumb" alt="">
            </figure>

            <h4 class="text">{{series}}</h4>
        </div>
            
    </div>
</template>

<script>
    export default {
        name: 'JumboCard',
        props: ['thumb', 'series'],
        data (){
            return{
            }
        }
    }
</script>

<style lang="scss" scoped>
     .card{
        width: calc((100% - 120px) / 6);
        display: flex;
        flex-direction: column;
        justify-content: space-between;
        align-items: center;
        flex-wrap: wrap;
        .thumb_wrapper{
            width: 250px;
            height: 280px;
            img{
                display: block;
                height: 100%;
                width: 100%;
                object-fit: cover;
                object-position: top;
            }
        }
        .text{
            margin-top: 10px;
            text-transform: uppercase;
            color: white;
            font-size: 15px;
            font-weight: 200;
            align-self: flex-start;
            white-space: nowrap;
            max-width: 15ch;
            
        }
    }
</style>