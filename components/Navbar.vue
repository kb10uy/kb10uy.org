<template>
  <header>
    <div class="container">
      <div class="left">
        <img src="~assets/img/tencocoa.png" alt="" class="logo" :class="{ extra: extraMode }" @click="clickLogo">
        <form action="https://www.google.com/search" method="get">
          <input type="hidden" name="q" value="kb10uy">
          <span class="search">
            <span class="hint">With kb10uy</span>
            <input type="text" name="q" class="query">
          </span>
        </form>
        <ul class="menu">
          <li>
            <a href="https://blog.kb10uy.org">Blog</a>
          </li>
          <li>
            <a href="https://ss.kb10uy.org">ShortStoryServer</a>
          </li>
          <li>
            <a href="https://streaming.kb10uy.org">Soine Streaming</a>
          </li>
        </ul>
      </div>
      <div class="right">
        <div class="personal">
          <img src="~assets/img/tenko-yaplus.png" alt="avatar" class="avatar" @click="toggleSocialLinks">
          <div class="dropdown" :class="{ hidden: !socialLinks }">
            <div class="head">kb10uy on</div>
            <hr>
            <ul class="social">
              <li><a href="https://mstdn.maud.io/@kb10uy">Mastodon (mstdn.maud.io)</a></li>
              <li><a href="https://twitter.com/kb10uy">Twitter</a></li>
              <li><a href="https://github.com/kb10uy">GitHub</a></li>
              <li><a href="http://steamcommunity.com/id/kb10uy">Steam</a></li>
              <li><a href="https://www.pixiv.net/member.php?id=4663583">pixiv</a></li>
            </ul>
          </div>
        </div>
      </div>
    </div>
  </header>
</template>

<style lang="scss">
header {
  background: #162249;
  padding: 4px 0;

  .container {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
  }

  .left {
    display: flex;
    align-items: center;

    .logo {
      width: 40px;
      height: 40px;

      &.extra {
        animation: rotation 0.5s linear infinite;
      }
      @keyframes rotation {
        0% {
          transform: rotateZ(0deg);
        }
        100% {
          transform: rotateZ(1080deg);
        }
      }
    }
  }

  .menu {
    color: #eeeeff;
    font-weight: bold;
    list-style: none;
    letter-spacing: -1em;
    margin: 0;
    padding: 0;

    li {
      display: inline-block;
      letter-spacing: normal;

      a {
        padding: 0 0.6em;
        text-decoration: none;
        color: #649464;
        &:hover {
          color: #a8d8a8;
        }
      }
    }
  }

  .search {
    letter-spacing: -1em;
    color: #cddbff;
    margin: 0 1em;

    .hint {
      border: 0;
      border-radius: 4px 0 0 4px;
      padding: 6px;
      margin-right: 1px;
      min-height: 24px;
      font-size: 13px;
      color: #cddbff;
      background-color: #3a3a6b;
      letter-spacing: normal;

      &:hover {
        background-color: #59598b;
      }
    }

    .query {
      border: 0;
      border-radius: 0 4px 4px 0;
      padding: 6px;

      font-size: 13px;
      font-family: 'Ubuntu', sans-serif;
      color: #cddbff;
      background-color: #3a3a6b;
      letter-spacing: normal;

      &:focus {
        outline: none;
      }
    }
  }

  .right {
    display: flex;
    align-items: center;

    .personal {
      position: relative;

      .dropdown {
        border: 1px solid #b4d6b4;
        border-radius: 4px;
        position: absolute;
        width: 200px;
        right: 0;
        top: 48px;
        background-color: #e9ffdf;
        box-shadow: 0px 0px 12px 4px rgba(0, 0, 0, 0.2);

        .head {
          font-size: 1.5em;
          font-weight: bold;
          padding: 8px;
        }

        hr {
          padding: 0;
          margin: 0;
          border: 0;
          border-top: 1px solid #b4d6b4;
        }
      }
    }

    .social {
      list-style: none;
      margin: 0;
      padding: 0;

      li a {
        display: block;
        text-decoration: none;
        padding: 8px;
        color: #649464;

        &:hover {
          display: block;
          text-decoration: none;
          padding: 8px;
          color: #eeffee;
          background-color: #32682a;
        }
      }
    }

    .avatar {
      border: 1px solid #111111;
      border-radius: 4px;
      width: 32px;
      height: 32px;
    }
  }
}
</style>

<script>
export default {
  data() {
    return {
      socialLinks: false,
      extraMode: false,
      logo: 0,
    };
  },

  methods: {
    toggleSocialLinks() {
      this.socialLinks = !this.socialLinks;
    },
    clickLogo() {
      this.logo++;
      if (this.logo >= 10) {
        this.extraMode = true;
      }
    },
  },
};
</script>
