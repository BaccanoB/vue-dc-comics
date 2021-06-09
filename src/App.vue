<template>
  <div id="app">
    <Header />
    <Main />
    <Footer />
  </div>
</template>

<script>
  import Header from './components/Header';
  import Main from './components/Main';
  import Footer from './components/Footer';
  export default{
    name:'App',
    components:{
      Header:Header,
      Main:Main,
      Footer:Footer
    }
  }
</script>

<style lang="scss">
@import './style/general';
</style>
