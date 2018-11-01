<template>
  <div class="aws-header">
    <span class="logo">KWS</span>
    <div class="menu">
      <nuxt-link to="#" class="menu-link">製品</nuxt-link>
      <nuxt-link to="#" class="menu-link">ソリューション</nuxt-link>
      <nuxt-link to="#" class="menu-link">料金表</nuxt-link>
      <nuxt-link to="#" class="menu-link">知識</nuxt-link>
      <nuxt-link to="#" class="menu-link">より詳しく</nuxt-link>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.aws-header {
  display: grid;
  grid-template-columns: max-content max-content 1fr max-content;
  align-items: center;
  padding: 2px 40px;
  background-color: #2a2a5c;
  color: #eee;

  .logo {
    font-size: 32pt;
  }

  .menu {
    display: flex;
    flex-direction: row;
    padding: 0;
    margin: 0;
    padding-left: 16px;

    .menu-link {
      display: inline-block;
      padding: 16px;
      text-decoration: none;
      color: inherit;
      &:hover {
        color: #f92;
      }
    }
  }
}
</style>


<script>
import Vue from 'vue';

export default Vue.extend({});
</script>
