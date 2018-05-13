<template>
  <div class="md-content">
    <div class="head">
      <slot name="title"></slot>
    </div>
    <div class="body">
      <slot></slot>
    </div>
  </div>
</template>

<style lang="scss" scoped>
$frame-color: #ffd5fc;
$header-bg-color: #fdf3fd;
$header-color: #b47fb0;
$body-bg-color: #ffffff;
$link-color: #97368f;

.md-content {
  margin: 8px 0;

  .head {
    padding: 8px;
    border: 1px solid $frame-color;
    border-radius: 4px 4px 0 0;
    background-color: $header-bg-color;
    // color: $header-color;
    // font-weight: bold;
  }

  .body {
    padding: 16px;
    border: solid $frame-color;
    border-width: 0px 1px 1px 1px;
    border-radius: 0 0 4px 4px;
    background-color: $body-bg-color;

    .center {
      text-align: center;
    }

    h1,
    h2 {
      margin: 1rem 0;
      padding-bottom: 0.3em;
      border-bottom: 1px solid $frame-color;
    }

    h3 {
      margin: 0.4em 0;
    }

    a {
      text-decoration: none;
      color: $link-color;
      &:hover {
        text-decoration: underline;
      }
    }

    li {
      line-height: 1.5em;
    }
  }
}
</style>

