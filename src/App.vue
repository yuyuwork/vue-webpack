<template>
  <div id="app">
    <img src="./assets/logo.png">
    <router-view/>
  </div>
</template>

<script>
export default {
  name: 'App'
}
</script>

// 使用@import引入外部css，作用域是全局的，也可在相应的单vue组件引入，
// import并不是引入代码到<style></style>里面，而是发起新的请求获得样式资源，
// 并且没有加scoped
// 注：如果有样式时，应该放在#app上面引入，不然引入不成功！
// @import改成<style src=""></style>引入外部样式
//@import "../static/css/animate.min.css";
<style>
body{
  margin:0px;
}
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
