<template>
  <div class="directory-table">
    <slot />
  </div>
</template>

<style lang="scss" scoped>
$frame-color: #ffd5fc;
$header-bg-color: #fdf3fd;
$table-content-color: #97368f;
$body-bg-color: #ffffff;
$table-message-color: #6d6d6d;

.directory-table {
  margin: 8px 0;

  .head {
    border: solid $frame-color;
    border-width: 1px 1px 0 1px;
    border-radius: 4px 4px 0 0;
    background-color: $header-bg-color;
    padding: 8px;
  }

  table {
    width: 100%;
    border-collapse: collapse;
    box-sizing: border-box;

    tr {
      background-color: $body-bg-color;
      border: 1px solid $frame-color;
      font-size: 11pt;
      &:hover {
        background-color: $header-bg-color;
      }
    }

    td {
      padding: 8px;
      &.icon {
        width: 1em;
        padding-right: 0;
      }
      &.content {
        width: 25%;
        a {
          text-decoration: none;
          color: $table-content-color;
          &:hover {
            text-decoration: underline;
          }
        }
      }
      &.message {
        color: $table-message-color;
      }
    }
  }
}
</style>

