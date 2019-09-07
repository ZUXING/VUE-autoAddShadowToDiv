# VUE-autoAddShadowToDiv

这是一个自带阴影的DIV标签，并整合为VUE组件的形式。
自定义长度、高度
只能使用一行文字，否则会溢出，高度和行高一样高
支持自定义阴影偏移量

代码示例：
<template>
  <div id="app">
    <shadowBox content="台灯" width="200" height="40" shifting="5" selected="selected"/>
    <!--
    	content="阴影盒子的内容"
    	width="宽度（单位：像素）"
    	height="高度（单位：像素）"
    	shifting="偏移量（单位：像素）"
    	selected="被选中的状态（尚未实现）"

    	使用时请手动给shadowBox插件留出它应有的高度值
    	否则在浏览器中shadowBox插件本身的高度值是0
    -->
  </div>
</template>

<script>
import shadowBox from './components/shadowBox.vue'

export default {
  name: 'app',
  components: {
    shadowBox
  }
}
</script>

刁♥陈
加油，刁，早日找到好工作！
