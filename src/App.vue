<template>
  <div id="app">
    <Header />
    <div id="head">
      <div class="head">
        <!-- <Header /> -->
        <header-sec></header-sec>
        <about-us></about-us>
      </div>      
    </div>    
    <simple-process></simple-process>
    <Services />
    <Strategia />
    <Products />
    <Footer />
  </div>
</template>

<script>
import Header from './components/Header'
import SimpleProces from './components/SimpleProcess'
import Services from './components/Services'
import HeaderSec from './components/HeaderSec'
import AboutUs from './components/AboutUs'
import Strategia from './components/Strategia'
import Products from './components/Products'
import Footer from './components/Footer'

export default {
  name: 'App',
  components: {
    Header,
    Services,
    Footer,
    Strategia,
    Products,
    'simple-process': SimpleProces,
    'header-sec': HeaderSec,
    'about-us': AboutUs
  }
}
</script>

<style>
  body {
    margin: 0;
    min-width: 320px;
    background-color: rgb(238, 238, 238);
    /* font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif; */
  }
  body::-webkit-scrollbar { width: 10px }
  body::-webkit-scrollbar-thumb { background: rgb(136, 136, 136) }
  body::-webkit-scrollbar-track { background: rgb(241, 241, 241) }
  #head {
    background-image: url('./assets/woman.jpg');
    background-attachment: fixed;
    background-repeat: no-repeat;
    background-size: cover;
    background-position: 0 50%;
  }
  .head { background-color: rgba(0, 0, 0, 0.5) }
  @media screen and (max-width: 576px) {
    #head {
      background-position: center
    }
  }
</style>
