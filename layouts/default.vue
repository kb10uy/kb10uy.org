<template>
  <div class="default-layout">
    <navbar />
    <nuxt />
    <my-footer />
  </div>
</template>

<style lang="scss">
$body-background: #e9ffdf;

.default-layout {
  background-color: $body-background;
  font-family: 'Ubuntu', sans-serif;
}

.container {
  margin: 0 auto;
  max-width: 1024px;
}

.hidden {
  display: none !important;
}
</style>

<script>
import Navbar from '~/components/Navbar.vue';
import MyFooter from '~/components/Footer.vue';

export default {
  components: {
    Navbar,
    MyFooter,
  },
};
</script>
