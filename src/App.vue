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
 </div>
</template>

<script>
import HeaderBox from './components/HeaderBox.vue'
import JumbotronBox from './components/JumbotronBox.vue'
import MainSection from './components/MainSection.vue'
import BlueSection from './components/BlueSection.vue'

export default {
  name: 'App',
  components: {
    // dichiaro componenti che utilizzerò
    HeaderBox,
    JumbotronBox,
    MainSection,
    BlueSection,

  }
}
</script>

<style lang="scss">
// importo main scss
@import './style/main.scss'
</style>
