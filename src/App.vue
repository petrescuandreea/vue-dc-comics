<template>
  <div id="app">
    <!-- componente Header  -->
    <Header/>

    <!-- componente jumbo  -->
    <Jumbo/>
    
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
import Jumbo from './components/Jumbo.vue';
import ComicSeries from './components/ComicSeries.vue';
import Footer from './components/Footer.vue';

export default {
  name: 'App',
  components: {
    Header,
    Jumbo,
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

  $brand_primary: #0282f9;

  header{
    a{
      &.active, &:hover{
          border-bottom: 4px solid $brand_primary;
          color: $brand_primary;
      }
    }
  }

  section {
    .title-wrapper {
      background-color: $brand_primary;
    }

    .btn-container {
      .btn-load-more {
        background-color: $brand_primary;
      }
    }
  }

    
}


</style>
