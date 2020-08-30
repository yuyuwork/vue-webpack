<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <ul>
      <li>
        <a
          href="https://vuejs.org"
          target="_blank"
        >
          Core Docs
        </a>
      </li>
    </ul>
  </div>
</template>

<script>
//http://shouce.jb51.net/velocity/
import { velocity } from '../../static/js/velocity.min.js'

//想在Vue组件中想要引入Velocity函数，那么要在Velocity加密算法的js脚本的最后，使用如下代码，将Velocity函数导出
//注：外部脚本js不要放在components文件夹下，否则会一直报错。可以在src文件夹下新建一个js文件夹，然后将外部js脚本放在这个文件夹下，然后就可以在其他Vue组件中引入该js脚本
//在组件中使用import { 函数名 } from 外部脚本名来从外部js脚本中导入我们需要使用的函数
//在Vue组件中正常调用Velocity函数
export default {
  name: 'HelloWorld',
  velocity,
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}

var encode = function (string) {
  // 这里是Velocity的具体实现算法
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
