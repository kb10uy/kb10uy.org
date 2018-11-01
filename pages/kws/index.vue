<template>
  <section>
    <aws-jumbotron>
      <h1>限界オタクの未来がここに</h1>
      <div class="summary">
        kb10uy へ移行し性癖のトランスフォーメーション（変革）をはじめるメリットと手順をご紹介
      </div>
    </aws-jumbotron>

    <aws-wrap>
      <h1>製品を調べる</h1>
      <h2><nuxt-link :to="{ name: 'kws-ec2' }">kb10uy EC2</nuxt-link></h2>
      <h2><nuxt-link :to="{ name: 'kws-s3' }">kb10uy S3</nuxt-link></h2>
    </aws-wrap>
  </section>
</template>

<script>
import Vue from 'vue';
import AwsServiceHeader from '~/components/aws/AwsServiceHeader.vue';
import AwsJumbotron from '~/components/aws/AwsJumbotron.vue';
import AwsWrap from '~/components/aws/AwsWrap.vue';

export default Vue.extend({
  layout: 'aws',
  components: {
    AwsServiceHeader,
    AwsJumbotron,
    AwsWrap,
  },

  head() {
    return {
      title: 'kb10uy EC2 (性的かつスケーラブルなオナホール上の仮想ペニスホスティング) | KWS',
    }
  }
});
</script>
