<script>
export default {
  name: 'jumbo',
};
</script>
<template>
  <!-- sezione Jumbo -->
  <section>
    <!-- container jumbo -->
    <div class="container">
      <h2>--content goes here --</h2>
    </div>
  </section>
  <!-- sezione Jumbo -->
</template>
<style scoped lang="scss">
@use '../style/partials' as *;

section {
  background-color: #1c1c1c;
  .container {
    padding: 50px 0;
    h2 {
      color: white;
      font-size: 30px;
    }
  }
}
</style>
