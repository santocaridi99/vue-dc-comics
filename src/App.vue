<template>
 <div id="app">
   <!-- sezione componente  HeaderBox -->
   <header-box></header-box>
   <!-- sezione jumbotron -->
   <jumbotron-box></jumbotron-box>
 </div>
</template>

<script>
import HeaderBox from './components/HeaderBox.vue'
import JumbotronBox from './components/JumbotronBox.vue'

export default {
  name: 'App',
  components: {
    // dichiaro componenti che utilizzerò
    HeaderBox,
    JumbotronBox
  }
}
</script>

<style lang="scss">
// importo main scss
@import './style/main.scss'
</style>
