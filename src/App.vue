<template>
 <div id="app">
   <!-- sezione componente  HeaderBox -->
   <header-box></header-box>
   <!-- sezione jumbotron -->
   <jumbotron-box></jumbotron-box>
   <!-- sezione main -->
   <main-section></main-section>
   <!-- sezione blu -->
   <blue-section></blue-section>
   <!-- sezione footer start -->
   <footer-start></footer-start>
   <!-- sezione footer end -->
   <footer-end></footer-end>
 </div>
</template>

<script>
// importo componenti 
import HeaderBox from './components/HeaderBox.vue'
import JumbotronBox from './components/JumbotronBox.vue'
import MainSection from './components/MainSection.vue'
import BlueSection from './components/BlueSection.vue'
import FooterStart from './components/FooterStart.vue'
import  FooterEnd from './components/FooterEnd.vue'

export default {
  name: 'App',
  components: {
    // dichiaro componenti che utilizzerò
    HeaderBox,
    JumbotronBox,
    MainSection,
    BlueSection,
    FooterStart,
    FooterEnd

  }
}
</script>

<style lang="scss">
// importo main scss
@import './style/main.scss'
</style>
