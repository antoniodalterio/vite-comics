<script>
import Header from './components/Header.vue';
import Jumbo from './components/Jumbo.vue';
import FooterApp from './components/FooterApp.vue';
export default {
  data() {
    return {};
  },
  components: {
    Header,
    Jumbo,
    FooterApp,
  },
};
</script>

<template>
  <Header></Header>
  <Jumbo></Jumbo>
  <FooterApp></FooterApp>
</template>

<style scoped lang="scss">
@use 'style/partials' as *;
</style>
