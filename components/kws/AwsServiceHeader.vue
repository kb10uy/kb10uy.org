<template>
  <div class="service-header">
    <div class="wrap">
      <slot />
    </div>
  </div>
</template>

<style lang="scss" scoped>
.service-header {
  background-color: #eee;
  padding: 0 20px;

  .wrap {
    display: flex;
    flex-direction: row;
    align-items: center;
    margin: 0 auto;
    width: 100%;
    max-width: 1200px;

    .name {
      font-size: 12pt;
      margin-right: 20px;
    }

    .menu {
      display: flex;
      flex-direction: row;
      align-items: center;

      .link {
        box-sizing: border-box;
        display: block;
        padding: 10px;
        padding-bottom: 8px;
        font-size: 10pt;
        &.selected {
          color: #26c;
          border-bottom: 2px solid #26c;
        }
        &:hover {
          color: #26c;
        }
      }
    }
  }
}
</style>
