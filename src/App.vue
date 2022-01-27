<template>
 <div id="app">
   <!-- sezione componente  HeaderBox -->
   <header-box></header-box>
 </div>
</template>

<script>
import HeaderBox from './components/HeaderBox.vue'

export default {
  name: 'App',
  components: {
    // dichiaro componenti che utilizzerò
    HeaderBox
  }
}
</script>

<style lang="scss">
// importo main scss
@import './style/main.scss'
</style>
