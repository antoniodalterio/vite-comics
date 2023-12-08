<script>
import Header from './components/Header.vue';
import Jumbo from './components/Jumbo.vue';
export default {
  data() {
    return {};
  },
  components: {
    Header,
    Jumbo,
  },
};
</script>

<template>
  <Header></Header>
  <Jumbo><div class="bg"></div></Jumbo>
</template>

<style scoped lang="scss">
@use 'style/partials' as *;
</style>
