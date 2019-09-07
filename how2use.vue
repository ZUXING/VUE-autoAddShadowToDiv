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
