<template>
  <div id="app">
    <div class="nav">
      <router-link to="/">
        <img src="http://cdn.imm1.cn/Application/Home/Public/style/images/logo.png" alt>
      </router-link>
    </div>
    <router-view/>
  </div>
</template>

<style>
* {
  margin: 0;
  padding: 0;
  list-style: none;
}
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
.nav {
  width: 1280px;
  margin: 0 auto;
}
</style>
