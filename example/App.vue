<style lang="styl">
body {
  font-size: 15px;
}
</style>
<style lang="styl" scoped>
// @import '../src/styles/index.less';
nav {
  margin-bottom: 40px;

  ul {
    display: flex;
    flex-wrap: wrap;
  }
  li {
    display: inline-block;
  }
  li + li {
    border-left: solid 1px #bbb;
    padding-left: 10px;
    margin-left: 10px;
  }
}
.container {
  padding: 10px 40px 0;
}
.v-link-active {
  color: #bbb;
}
.split-box {
  padding: 0 15px;
}
</style>
<template>
  <div class="container">
    <nav>
      <ul>
        <li>
          <router-link to="/button">button</router-link>
          <span class="split-box">|</span>
          <router-link to="/date-picker">date-picker</router-link>
        </li>
      </ul>
    </nav>
    <router-view></router-view>
  </div>
</template>
<script>
module.exports = {
  data: function() {
    return {}
  }
}
</script>
