<template>
<!-- questo component si deve fare domani -->
    <main>
        <!-- contenitore carte -->
        <div class="card-container">
            <!-- per card presenti nell'array fumetti  creo classe card -->
            <div v-for="(card,i) in comics" :key='i' class="card">
                <!-- card avrà vari attributi dell'oggetto per immagine e per il text box(area di testo) -->
             <img :src="card.thumb" alt="card.series">
             <div class="text-box">{{card.series}}</div>
            </div> 
        </div>
        <!-- bottone in basso al main -->
        <div class="button-container">
            <button class="button more">LOAD MORE</button>
        </div>
    </main>
</template>
<script>
export default {
    // variabili che vengono passate dal padre(app)
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
    // contenitore carte
    .card-container{
        width: 1200px;
        margin: 0 auto;
        display: flex;
        justify-content: space-between;
        flex-wrap: wrap;
        padding: 60px;
        // carta
        .card{
            width:calc(100% / 6  - 20px);
            height: 280px;
            margin-left: 20px;
            margin-top: 10px;
            // immagine
            img{
                width: 100%;
                height: 80%;
            } 
            // area testo
            .text-box{
                color: $main-white-color;
                padding: 15px 0;
            }   
        }
      
    }
    // contenitore del bottone
    .button-container{
        width: 100%;
        display: flex;
        justify-content: center;
        padding: 30px;
        button{
            background-color: $main-color;
            color: $main-white-color;
            border: none;
            padding: 10px 40px;
            font-weight: bold;
        }
    }
    
}
</style>