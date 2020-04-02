<template>
  <div class="header_top">
    <slot name="logo"></slot>
    <router-link class="header_login" to="/login" tag="span">
      <span class="login_span">登录|注册</span>
    </router-link>
  </div>
</template>

<script>
export default {
  data () {
    return {}
  },
  methods: {},
  components: {}
}
</script>

<style lang="scss" scoped>
@import "../../style/mixin";
.header_top {
  position: fixed;
  background-color: $blue;
  top: 0;
  left: 0;
  height: 10%;
  width: 100%;

  .header_logo {
    float: left;
    width: 25%;
    height: 100%;
    img {
      height: 100%;
    }
  }

  .header_login {
    float: right;
    display: table;
    width: 30%;
    height: 100%;

    .login_span {
      color: #fff;
      font-size: 3rem;
      text-align: center;
      vertical-align: middle;
      display: table-cell;
    }
  }
}
</style>
