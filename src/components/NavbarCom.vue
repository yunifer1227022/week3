<template>
  <div class="navbar">
    <div class="container flex jcsb ai-center">
      <h1>
        <img
          src="https://github.com/hexschool/2022-web-layout-training/blob/main/week3-4/logo-white.png?raw=true"
          alt="logo"
        />
      </h1>
      <ul class="flex nav">
        <li><a href="#">系列鏡框</a></li>
        <li><a href="#">門市據點</a></li>
        <li><a href="#">部落格</a></li>
        <li><a href="#">常見問題</a></li>
      </ul>
    </div>
  </div>
</template>

<style lang="scss">
@import '../assets/base.scss';
.navbar {
  background: $primary;
  .flex {
    @include mobile {
      flex-direction: column;
      align-items: flex-start;
      max-width: 100%;
      padding: 0;
    }
  }
  h1 {
    width: 80px;
    margin: 12px 0;
    @include mobile {
      margin: 16px;
    }
  }
  .nav {
    @include mobile {
      flex-direction: row;
      flex-wrap: wrap;
      width: 100%;
    }
    li {
      vertical-align: middle;
      margin-left: 64px;
      @include mobile {
        font-size: 16px;
        text-align: center;
        border: 1px solid #fff;
        padding: 12px 0;
        margin-left: 0;
        width: 50%;
      }
      a {
        font-size: 20px;
        color: $white;
        padding: 25px 0px 25px 0px;
        @include mobile {
          padding: 0;
          width: 100%;
          height: 100%;
        }
      }
    }
  }
}
</style>
