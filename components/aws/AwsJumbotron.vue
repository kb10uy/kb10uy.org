<template>
<div class="jumbotron">
  <div class="wrap">
    <slot />
  </div>
</div>
</template>

<style lang="scss" scoped>
.jumbotron {
  padding: 0 20px;
  background-image: url('~assets/img/kws-jumbotron-back.jpg');
  background-size: cover;
  .wrap {
    align-items: center;
    margin: 0 auto;
    padding: 30px;
    width: 100%;
    max-width: 1200px;
    color: #fff;

    h1 {
      margin: 0;
      font-size: 40pt;
      line-height: 1.2;
      font-weight: 500;
    }

    .summary {
      box-sizing: border-box;
      margin: 8px 0;
      font-size: 18pt;
      &.with-box {
        padding: 15px;
        border-left: 3px solid #243;
      }
    }
  }
}
</style>
