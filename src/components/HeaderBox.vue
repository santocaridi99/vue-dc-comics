<template>
    <header>
        <div class="logo">
            <img src="@/assets/dc-logo.png" alt="">
        </div>
        <nav>
            <ul>
                <li>CHARACTERS</li>
                <li>COMICS</li>
                <li>MOVIES</li>
                <li>TV</li>
                <li>GAMES</li>
                <li>COLLECTIBLES</li>
                <li>VIDEOS</li>
                <li>FANS</li>
                <li>NEWS</li>
                <li>SHOP</li>
            </ul>
        </nav>
    </header>
</template>
<script>
export default {
    
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
            padding: 30px 10px;
            // hover della lista
            &:hover{
                color: $main-color;
                border-bottom: 5px solid #3297fb; 
                cursor: pointer;
            }
        }
    }


}
</style>