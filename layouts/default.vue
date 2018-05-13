<template>
  <div>
    <navbar />
    <nuxt />
  </div>
</template>

<style lang="scss">
$body-background: #e9ffdf;

body {
  margin: 0;
  padding: 0;
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

export default {
  components: {
    Navbar,
  },
};
</script>
