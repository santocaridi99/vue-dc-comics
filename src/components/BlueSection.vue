<template>
<!-- container blu con dentro una ul con li(immagine + testo span) -->
    <div class="container-blue">
        <ul>
            <li>
                <img src="@/assets/buy-comics-digital-comics.png" alt="buy comics">
                <span>DIGITAL COMICS</span>
            </li>
            <li>
                <img src="@/assets/buy-comics-merchandise.png" alt="dc merchandise">
                <span>DC MERCHANDISE</span>
            </li>
            <li>
                <img src="@/assets/buy-comics-subscriptions.png" alt="subscriptions">
                <span>SUBSCRIPTION</span>
            </li>
            <li>
                <img src="@/assets/buy-comics-shop-locator.png" alt="shop location">
                <span>COMIC SHOP LOCATOR</span>
            </li>
            <li>
                <img src="@/assets/buy-dc-power-visa.svg" alt="visa">
                <span>DC POWER VISA</span>
            </li>
        </ul>
    </div>
</template>
<script>
export default {
    
}
</script>
<style lang="scss" scoped>
@import '@/style/variables.scss';
// stile del contenitore blu con dentro lista di immagini + testo
.container-blue{
    background-color: $main-color;
    height: 25vh;
    width: 100%;
    ul{
        display: flex;
        height: 100%;
        justify-content: space-around;
        align-items: center;
        li{
            display: flex;
            align-items: center;
            cursor: pointer;
            img{
                width: 80px;
                height: 80px;
            }
            span{
                margin-left: 5px;
                color: $main-white-color;
            }
        }
    }
}
</style>