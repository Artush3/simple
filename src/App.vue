<script>
import Header from './components/Header/Header.vue';
import Main from './components/Main/Main.vue';
import Footer from './components/Footer/Footer.vue';
export default {
  name: "App",
  components: { Header, Main, Footer }
}
</script>

<template>
  <Header></Header>
  <Main></Main>
  <Footer></Footer>
</template>