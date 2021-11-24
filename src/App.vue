<template>
  <div id="app">
    <!-- componente Header  -->
    <Header/>

    <main>
      <!-- componente Conent  -->
      <Content/>
    </main>

    <footer>
      <!-- componente Footer  -->
      <Footer/>
    </footer>
  </div>
</template>

<script>
import Header from './components/Header.vue';
import Content from './components/Content.vue';
import Footer from './components/Footer.vue';

export default {
  name: 'App',
  components: {
    Header,
    Content,
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
  // text-align: center;
  // color: #2c3e50;
  // margin-top: 60px;
}

main {
  padding: 40px 0;
  background-color: rgba(28,28,28,255);
}
</style>
