<template>
  <div id="app">
    <header>猫眼电影</header>
    <main></main>
    <nav>
      <ul>
        <li class="active">
          <b>&#xe8ae;</b>
          <span>电影</span>
        </li>
        <li>
          <b>&#xe8c0;</b>
          <span>影院</span>
        </li>
        <li>
          <b>&#xe606;</b>
          <span>我的</span>
        </li>
      </ul>
    </nav>
  </div>
</template>

<script>
export default {
  data() {
    return {
      msg: "hello",
    };
  },
};
</script>

<style lang="stylus" scoped>
@font-face {
  font-family: iconfont-nav;
  src: url('./assets/icons/iconfont-nav.ttf') format('truetype');
}

div {
  display: flex;
  flex-direction: column;

  header {
    background-color: #cd4c42;
    color: #fff;
    height: 0.44rem;
    font-size: 0.16rem;
    font-weight: bold;
    text-align: center;
    line-height: 0.44rem;
  }

  main {
    flex: 1;
  }

  nav {
    height: 0.5rem;
    border-top: 1px solid #ededed;

    ul {
      display: flex;
      height 100%

      li {
        flex: 1;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        font-family: iconfont-nav;
        color: #999;

        b {
          font-size: 0.26rem;
          font-weight: normal;
          line-height: 0.25rem;
        }

        span {
          font-size: 0.12rem;
          transform: scale(0.9);
        }
      }

      .active {
        color: #cd4c42;
      }
    }
  }
}
</style>
