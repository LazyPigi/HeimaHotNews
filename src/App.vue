<template>
    <div>
      <!-- 组件占位符 -->
      <router-view></router-view>
    </div>
</template>

<script>
export default {
  data() {
    return {};
  }
};
</script>

<style>
/* 引入字体图标文件 */
@import url('../font_1426139_h6vn3jbl5q.css');
@import url("../node_modules/vant/lib/index.css");


/* 公共样式 */
html,body {
  background: #f6f6f6;
}

*{
  margin: 0;
  padding: 0;
}

a {
  color: inherit;
}

a:hover {
  text-decoration: none;
}

ul,li,ol {
  list-style: none;
}

i,em {
  font-size: normal;
}
</style>