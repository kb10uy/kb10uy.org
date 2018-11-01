<template>
  <div>
    <aws-header />
    <nuxt />
  </div>
</template>

<style lang="scss">
body {
  margin: 0;
  padding: 0;
  font-family: sans-serif;
}
</style>

<script>
import Vue from 'vue';
import AwsHeader from '~/components/aws/AwsHeader.vue';

export default Vue.extend({
  components: {
    AwsHeader,
  },
});
</script>
