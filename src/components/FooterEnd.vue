<template>
<!-- seconda parte del footer -->
    <div class="container-footer-end">
        <!-- bottone e un div con dentro le foto dei socials -->
        <button class="button sign-up">SIGN-UP NOW!</button>
        <div class="socials">
            <h3>FOLLOW US</h3>
            <img src="@/assets/footer-facebook.png" alt="facebook">
            <img src="@/assets/footer-twitter.png" alt="twitter">
            <img src="@/assets/footer-youtube.png" alt="yt">
            <img src="@/assets/footer-pinterest.png" alt="pinterest">                <img src="@/assets/footer-periscope.png" alt="periscope logo">
        </div>
    </div>
</template>
<script>
export default {
    
}
</script>
<style lang="scss" scoped>
@import '@/style/variables.scss';
// stile della seconda parte del container
.container-footer-end{
    background-color: $black-special;
    height: 15vh;
    width: 100%;
    display: flex;
    justify-content: space-around;
    align-items: center;
    // bottone interno
    button{
        color:$main-white-color;
        background-color: $black-special;
        padding: 15px;
        border:2px solid $main-color;
    }
    // contenitore dei socials con testo + img
    .socials{
        display: flex;
        align-items: center;
        h3{
            color: $main-color;
            margin-right: 10px;
        }
        img{
            padding: 0 5px;
        }
    }
}
</style>