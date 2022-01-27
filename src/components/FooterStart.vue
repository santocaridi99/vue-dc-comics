<template>
<!-- contenitore footer iniziale -->
    <div class="container-footer-start">
        <!-- nav bar con i vari div con titoli e liste -->
        <div class="footer-nav">
            <div class="comics-shop">
                <h3>DC COMICS</h3>
                <ul>
                    <li>Characters</li>
                    <li>Comics</li>
                    <li>Movies</li>
                    <li>Games</li>
                    <li>Videos</li>
                    <li>News</li>
                </ul>
                <h3>SHOP</h3>
                <ul>
                    <li>Shop DC</li>
                    <li>Shop DC Collectibles</li>
                </ul>
            </div>
            <div class="dc">
                <h3>DC</h3>
                <ul>
                    <li>Terms Of Use</li>
                    <li>Privacy policy (New)</li>
                    <li>ad Choices</li>
                    <li>Advertising</li>
                    <li>Jobs</li>
                    <li>Subscriptions</li>
                    <li>Talent Workshops</li>
                    <li>CPSC Certificates</li>
                    <li>Rating</li>
                    <li>Shop Help</li>
                    <li>Contact Us</li>
                </ul>
            </div>
            <div class="site">
                <h3>SITE</h3>
                <ul>
                    <li>DC</li>
                    <li>MAD Magazine</li>
                    <li>DC Kids</li>
                    <li>DC universe</li>
                    <li>DC Power Visa</li>
                </ul>
            </div>
        </div>
        <!-- logo di background -->
        <div class="bg-logo">
            <img src="../assets/dc-logo-bg.png" alt="">
        </div>
    </div>
</template>
<script>
export default {
    
}
</script>
<style lang="scss" scoped>
@import '@/style/variables.scss';
.container-footer-start{
    height: 40vh;
    width: 100%;
    background: url('../assets/footer-bg.jpg') no-repeat;
    background-size: cover;
    position: relative;
    padding: 20px 30px;
    // logo di background con relativa img
    .bg-logo{
        height: 50%;
        img{
            z-index: 1;
            width: 30%;
            height: 100%;
            position:absolute;
            right: 20%;
            bottom: -5%;
        }
    }
    .footer-nav{
        display: flex;
        div{
            margin: 15px;
            h3{
                color:$main-white-color;
                margin: 5px 0;
            }
            ul{
                li{
                    color:grey;
                    font-size: 12px;
                    cursor: pointer;
                    &:hover{
                        color: $main-white-color;
                    }
                }
            }
        }
    }
}
</style>