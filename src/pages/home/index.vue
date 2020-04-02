<template>
  <div class="posit_container">
      <header-top>
        <div slot="logo" class="header_logo">
          <img src="@/assets/logo.png" alt="elm">
        </div>
      </header-top>
      <nav class="city_nav">
        <section class="posit_header">
            <span class="left">当前定位城市：</span>
            <span class="right">定位不准时，请在城市列表中选择</span>
        </section>
        <router-link class="posit" to="/login" tag="section">
            <span class="left">南京</span>
            <span class="right">></span>
        </router-link>
      </nav>
      <section class="hot_city"></section>
      <section class="city_group"></section>
  </div>
</template>

<script>
import HeaderTop from '../../components/header'
export default {
  data () {
    return {

    }
  },
  methods: {

  },
  components: {
    HeaderTop
  }
}
</script>

<style lang="scss" scoped>
    @import '../../style/common';
    .city_nav {
        margin-top: 14%;
        height: 20%;
        border: 1px solid #000;

        .posit_header {
            height: 80px;
            width: 100%;
        }
    }
</style>
