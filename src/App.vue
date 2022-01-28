<template>
 <div id="app">
   <!-- sezione componente  HeaderBox -->
   <!-- assegno all'array nav uguale a list in headerbox -->
   <header-box :lists=navbar></header-box>
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

  },
  data(){
    return{
    // navbar
       navbar:[
        {
          id:'1',
          text:'CHARACTERS',
          url:'/'
        },
        {
          id:'2',
          text:'COMICS',
          url:'/'
        },
        {
          id:'3',
          text:'MOVIES',
          url:'/'
        },
        {
          id:'4',
          text:'TV',
          url:'/'
        },
        {
          id:'5',
          text:'GAMES',
          url:'/'
        },
        {
          id:'6',
          text:'COLLECTIBLES',
          url:'/'
        },
        {
          id:'7',
          text:'VIDEOS',
          url:'/'
        },
        {
          id:'8',
          text:'FANS',
          url:'/'
        },
        {
          id:'9',
          text:'NEWS',
          url:'/'
        },
        {
          id:'10',
          text:'SHOP',
          url:'/'
        },
      ]
    }
  }
}
</script>

<style lang="scss">
// importo main scss
@import './style/main.scss'
</style>
