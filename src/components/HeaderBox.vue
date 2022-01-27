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
header{
    // stile dell'header
    display: flex;
    width: 100%;
    justify-content: space-around;
    align-items: center;
    height: 25vh;
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
            list-style: none;
            padding: 30px 10px;
            // hover della lista
            &:hover{
                color: #107ae7;
                border-bottom: 3px solid #107ae7; 
                cursor: pointer;
            }
        }
    }


}
</style>