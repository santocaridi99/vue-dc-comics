<template>
    <header>
        <div class="logo">
            <img src="@/assets/dc-logo.png" alt="">
        </div>
        <nav>
            <ul>
                <!-- per ogni list presente nell'array lists che corrisponde all'array navbar in App -->
                <!-- creo delle li con chiave id-->
                <!-- con un link a con url e testo -->
                <li v-for='list in lists' :key='list.id'>
                    <a :href="list.url">
                        {{list.text}}
                    </a>
                </li>
            </ul>
        </nav>
    </header>
</template>
<script>
export default {
    // variabili che vengono passate dal padre(app)
    props:{
        lists:Array,
    }
    
}
</script>
<style lang="scss" scoped>
@import '@/style/variables.scss';
header{
    // stile dell'header
    display: flex;
    width: 100%;
    justify-content: space-around;
    align-items: center;
    height: 15vh;
    // container logo
    .logo{
        width: 60px;
        height: 60px;
        // grandezza immagine dentro logo
        img{
            width: 100%;
        }
    }
    // lista
    ul{
        display: flex;
        li{
            padding: 0px 10px;
            a{
                color:black ;
                &:hover{
                    // hover ai link
                    color: $main-color;
                    padding: 30px 0;
                    border-bottom: 5px solid #3297fb; 
                }
            }
        }
    }


}
</style>