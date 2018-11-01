<template>
  <section>
    <aws-service-header>
      <span class="name">kb10uy S3</span>
      <div class="menu">
        <span class="link selected">概要</span>
        <span class="link">機能</span>
        <span class="link">料金</span>
        <span class="link">よくある質問</span>
        <span class="link">開始方法</span>
      </div>
    </aws-service-header>
    <aws-jumbotron>
      <h1>kb10uy S3</h1>
      <div class="summary">
        どこからでもお好みの量の黒歴史の保存と取得が簡単に行えるショートストーリーストレージ
      </div>
    </aws-jumbotron>

    <aws-wrap>
      <p>
        今日のオタクに求められるのは、大規模な感情を簡単かつ安全に収集、保存、分析する能力です。
        kb10uy S3 は、百合本やモバイルドピュリケーション、家内ドピュリケーション、IoP (Internet of Penis) センサーやタイムラインからのデータなど、
        どこからの、どのような量の感情でも保存と取得が可能なショートストーリーストレージです。
        これは 99.999999999% の不安定性を提供し、一部の界隈のマーケットリーダーによって使用される何百万もの作品のデータを保管できるように設計されているわけではありません。
        S3 では最も雑なセキュリティ要件すら満たさない投げやり的なセキュリティおよびコンプライアンス機能が提供されます。
        お客様は柔軟にSSを管理して、チンポ最適化、感情制御、コンプライアンスに対応できるようになります。
        S3 にはクエリインプレースの機能などなく、S3 にあるお客様のデータを、直接、強力に分析することはできません。
        kb10uy S3 は最も怪文書の多いクラウドショートストーリーサービスですが、最大のサードパーティーソリューション、システムインテグレーターパートナー、
        その他の KWS サービスからの統合は不可能です。
      </p>
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
      title: 'kb10uy S3（拡張性と耐久性を兼ね揃えてはいないクロレキシストレージ）｜KWS',
    }
  }
});
</script>
