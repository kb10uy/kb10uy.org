<template>
  <div class="container">
    <directory-table>
      <div class="head">
        Contents
      </div>
      <table>
        <tbody>
          <tr>
            <td class="icon">📁</td>
            <td class="content"><a href="https://blog.kb10uy.org">blog</a></td>
            <td class="message">My blog</td>
          </tr>
          <tr>
            <td class="icon">📁</td>
            <td class="content"><a href="https://ss.kb10uy.org">ss</a></td>
            <td class="message">ShortStoryServer (under construction)</td>
          </tr>
          <tr>
            <td class="icon">📁</td>
            <td class="content"><a href="https://streaming.kb10uy.org">streaming</a></td>
            <td class="message">Soine Streaming Server</td>
          </tr>
          <tr>
            <td class="icon">📁</td>
            <td class="content"><a href="https://files.kb10uy.org">files</a></td>
            <td class="message">Autoindex of this site (original design)</td>
          </tr>
          <tr>
            <td class="icon">📁</td>
            <td class="content"><a href="https://seaurchin.kb10uy.org">seaurchin</a></td>
            <td class="message">Seaurchin Wiki</td>
          </tr>
          <tr>
            <td class="icon">📁</td>
            <td class="content"><a href="http://homo.kb10uy.org">homo</a></td>
            <td class="message">The ring of victim of @mpyw</td>
          </tr>
          <tr>
            <td class="icon">↩</td>
            <td class="content"><a href="http://xn--ydko.kb10uy.org">ホモ</a></td>
            <td class="message">Alias of homo</td>
          </tr>
          <tr>
            <td class="icon">📁</td>
            <td class="content"><a href="http://mpyw.kb10uy.org">mpyw</a></td>
            <td class="message">@mpyw lootbox</td>
          </tr>
          <tr>
            <td class="icon">📁</td>
            <td class="content"><a href="http://api.mpyw.kb10uy.org">api.mpyw</a></td>
            <td class="message">@mpyw lootbox API</td>
          </tr>
          <tr>
            <td class="icon">📁</td>
            <td class="content"><a href="https://databaseerror.kb10uy.org">databaseerror</a></td>
            <td class="message">Error establishing a database connection</td>
          </tr>
          <tr>
            <td class="icon">↩</td>
            <td class="content"><a href="https://xn--ick7ar5azg9dxfcd1080khq1bngf9qk.kb10uy.org">データベース接続確立エラー</a></td>
            <td class="message">Alias of databaseerror</td>
          </tr>
          <tr>
            <td class="icon">📁</td>
            <td class="content"><a href="http://sperm.kb10uy.org">sperm</a></td>
            <td class="message">My used condom</td>
          </tr>
          <tr>
            <td class="icon">↩</td>
            <td class="content"><a href="http://xn--cbktfsc9d4d8b6925a0bxc9nn.kb10uy.org">使用済みコンドーム</a></td>
            <td class="message">Alias of sperm</td>
          </tr>
          <tr>
            <td class="icon">↩</td>
            <td class="content"><a href="http://xn--ick7ar5azg9dxfcd1080khq1bngf9qk.kb10uy.org">σπέρμα</a></td>
            <td class="message">Alias of sperm</td>
          </tr>
          <tr>
            <td class="icon">📁</td>
            <td class="content"><a href="http://hydrogen-sound.kb10uy.org">hydrogen-sound</a></td>
            <td class="message">Ah, the sound of hydrogen!</td>
          </tr>
          <tr>
            <td class="icon">↩</td>
            <td class="content"><a href="http://xn--1rwa901k.kb10uy.org">水素水</a></td>
            <td class="message">Alias of hydrogen-sound</td>
          </tr>
          <tr>
            <td class="icon">📁</td>
            <td class="content"><a href="http://hydrogen-sound.kb10uy.org">api.hydrogen-sound</a></td>
            <td class="message">Hydrogen sound API</td>
          </tr>
          <tr>
            <td class="icon">📁</td>
            <td class="content"><a href="https://netdata.kb10uy.org">netdata</a></td>
            <td class="message">The netdata status</td>
          </tr>
          <tr>
            <td class="icon">📁</td>
            <td class="content"><a href="https://ontology.kb10uy.org">ontology</a></td>
            <td class="message">Screenshots of my SSR idols</td>
          </tr>
        </tbody>
      </table>
    </directory-table>

    <md-content>
      <span slot="title">Server Status</span>
      <div class="center">
        <img src="~assets/img/tencocoa.png" alt="kb10uy.org logo" class="logo" width="200">
        <br>
        <a class="badge" href="https://netdata.kb10uy.org/#menu_system_submenu_cpu"><img alt="CPU Usage" src="https://netdata.kb10uy.org/api/v1/badge.svg?chart=system.cpu&label=CPU+Usage&units=%25"></a>
        <a class="badge" href="https://netdata.kb10uy.org/#menu_system_submenu_load"><img alt="Load Average" src="https://netdata.kb10uy.org/api/v1/badge.svg?chart=system.load&dimensions=load5&label=Load+Average&units=null"></a>
        <a class="badge" href="https://netdata.kb10uy.org/#menu_sensors_submenu_temperature"><img alt="CPU Temperature" src="https://netdata.kb10uy.org/api/v1/badge.svg?chart=sensors.pch_skylake_virtual_0_temperature&label=CPU+Temperature&units=+%27C"></a>
        <a class="badge" href="https://netdata.kb10uy.org/#menu_net_submenu_enp0s31f6"><img alt="Outbound" src="https://netdata.kb10uy.org/api/v1/badge.svg?chart=net.enp0s31f6&dimension=sent&label=Outbound&options=abs"></a>
        <a class="badge" href="https://netdata.kb10uy.org/#menu_system_submenu_uptime"><img alt="Uptime" src="https://netdata.kb10uy.org/api/v1/badge.svg?chart=system.uptime&label=Uptime&value_color=blue"></a>
      </div>
      <h1>kb10uy.org</h1>
      The design of this site is heavily inspired by GitHub.
    </md-content>
  </div>
</template>

<style lang="scss" scoped>
.badge {
  margin: 0 0.4em;
}
</style>


<script>
import MdContent from '~/components/MdContent.vue';
import DirectoryTable from '~/components/DirectoryTable.vue';

export default {
  components: {
    MdContent,
    DirectoryTable,
  },
  mounted() {
    const consoleMessageStyle = `
      font: 20pt monospace;
      color: #f2f;
    `;
    console.log('%cI am dopyulicating!', consoleMessageStyle);
  },

  head() {
    return {
      title: 'Top',
    };
  },
};
</script>
