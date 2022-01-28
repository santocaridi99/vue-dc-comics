<template>
<!-- questo component si deve fare domani -->
    <main>
        <div class="card-container">
            <div v-for="(card,i) in comics" :key='i' class="card">
             <img :src="card.thumb" alt="card.series">
             <div class="text-box">{{card.series}}</div>
            </div>
           
        </div>
    </main>
</template>
<script>
export default {
    props:{
        comics:Array,
    }
}
</script>
<style lang="scss" scoped>
@import '@/style/variables.scss';
main{
    // style da fare domani
    width: 100%;
    background-color:$black-special;
    .card-container{
        width: 1200px;
        margin: 0 auto;
        display: flex;
        justify-content: space-between;
        flex-wrap: wrap;
        padding: 60px;
        .card{
            width:calc(100% / 6  - 20px);
            height: 280px;
            margin-left: 20px;
            img{
                width: 100%;
                height: 80%;
            } 
            .text-box{
                color: $main-white-color;
                padding: 15px 0;
            }   
        }
      
    }
    
}
</style>