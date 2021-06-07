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
  @import url('https://fonts.googleapis.com/css2?family=Open+Sans+Condensed:wght@300;700&display=swap');
  body {
    font-family: 'Open Sans Condensed', sans-serif;
  }
  * {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
}

</style>
