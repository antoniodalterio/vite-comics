<script>
import Header from './components/Header.vue';
import ContentMain from './components/ContentMain.vue';
import NavBar from './components/NavBar.vue';
import FooterApp from './components/FooterApp.vue';

export default {
  data() {
    return {};
  },
  components: {
    Header,
    ContentMain,
    NavBar,
    FooterApp,
  },
};
</script>

<template>
  <Header></Header>
  <ContentMain></ContentMain>
  <NavBar></NavBar>
  <FooterApp></FooterApp>
</template>

<style scoped lang="scss">
@use 'style/partials' as *;
</style>
