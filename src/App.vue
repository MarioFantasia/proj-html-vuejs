<template>
  <div id="app">
    <Header></Header>
    <Main></Main>
    <Footer></Footer>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Main from './components/Main.vue'
import Footer from './components/Footer.vue'
export default {
  /* componenti App */
  components : {
    Header,
    Main,
    Footer
  }
}
</script>

<style lang="scss">
  /* importo fontawesome */
  @import '~@fortawesome/fontawesome-free/css/all.css';
/* importo il file common.scss */
  @import './assets/style/common.scss';

</style>
