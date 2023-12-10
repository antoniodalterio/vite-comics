<script>
import Header from './components/Header.vue';
import Jumbo from './components/Jumbo.vue';
import ContentMain from './components/ContentMain.vue';
import FooterApp from './components/FooterApp.vue';

export default {
  data() {
    return {};
  },
  components: {
    Header,
    Jumbo,
    ContentMain,
    FooterApp,
  },
};
</script>

<template>
  <Header></Header>
  <Jumbo></Jumbo>
  <ContentMain></ContentMain>
  <FooterApp></FooterApp>
</template>

<style scoped lang="scss">
@use 'style/partials' as *;
</style>
