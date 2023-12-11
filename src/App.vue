<script>
import Header from './components/Header.vue';
import Jumbo from './components/Jumbo.vue';
import ContentMain from './components/ContentMain.vue';
import NavBar from './components/NavBar.vue';
import FooterApp from './components/FooterApp.vue';

export default {
  data() {
    return {};
  },
  components: {
    Header,
    Jumbo,
    ContentMain,
    NavBar,
    FooterApp,
  },
};
</script>

<template>
  <Header></Header>
  <Jumbo></Jumbo>
  <ContentMain></ContentMain>
  <NavBar></NavBar>
  <FooterApp></FooterApp>
</template>

<style scoped lang="scss">
@use 'style/partials' as *;
</style>
