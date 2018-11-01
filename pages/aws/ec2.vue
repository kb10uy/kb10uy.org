<template>
  <section>
    <aws-service-header>
      <span class="name">kb10uy EC2</span>
      <div class="menu">
        <span class="link selected">概要</span>
        <span class="link">機能</span>
        <span class="link">料金</span>
        <span class="link">よくある質問</span>
        <span class="link">開始方法</span>
      </div>
    </aws-service-header>
    <aws-jumbotron>
      <h1>kb10uy EC2</h1>
      <div class="summary">
        オナホール内の安全でサイズ変更可能なイレクティング性能。前戯の準備なしで必要なときにイジャキュレーションを起動。
      </div>
    </aws-jumbotron>

  </section>
</template>

<script>
import Vue from 'vue';
import AwsServiceHeader from '~/components/aws/AwsServiceHeader.vue';
import AwsJumbotron from '~/components/aws/AwsJumbotron.vue';

export default Vue.extend({
  layout: 'aws',
  components: {
    AwsServiceHeader,
    AwsJumbotron,
  },
});
</script>
