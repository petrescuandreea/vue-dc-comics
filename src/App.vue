<template>
  <div id="app">
    <!-- componente Header  -->
    <Header/>

    <main>
      <!-- componente Conent  -->
      <ComicSeries/>
    </main>

    <footer>
      <!-- componente Footer  -->
      <Footer/>
    </footer>
  </div>
</template>

<script>
import Header from './components/Header.vue';
import ComicSeries from './components/ComicSeries.vue';
import Footer from './components/Footer.vue';

export default {
  name: 'App',
  components: {
    Header,
    ComicSeries,
    Footer
  }
}
</script>

<style lang="scss">
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}


</style>
