<template>
  <div>
    <ul>
      <li class="submenu">
        <a href="#">云技术管理</a>
        <ul>
          <li>
            <a href="#">云服务器</a>
          </li>
          <li>
            <a href="#">云数据库</a>
          </li>
          <li>
            <a href="#">负载均衡</a>
          </li>
        </ul>
      </li>
    </ul>
    <ul>
      <li class="submenu">
        <a href="#">安全管理</a>
        <ul>
          <li>
            <a href="#">云盾控制台</a>
          </li>
          <li>
            <a href="#">DDoS高防IP</a>
          </li>
          <li>
            <a href="#">Web应用防火墙</a>
          </li>
          <li>
            <a href="#">CA证书服务</a>
          </li>
        </ul>
      </li>
    </ul>
  </div>
</template>
<style scoped>
div {
  padding: 5px;
  display: inline-block;
  vertical-align: top;
  width: 230px;
  border: 1px solid red;
  margin: 5px 10px;
}
/* 一二级ul样式 */
ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
  background-color: #f1f1f1;
}
/* 一二级超链接导航样式 */
a {
  display: block;
  color: #000;
  padding: 8px 16px;
  text-decoration: none;
}
/* 一级标题 */
li.submenu > a {
  background-color: #333;
  font-weight: bold;
  color: #1d835a;
}
a:hover {
  font-weight: bold;
  background-color: #555;
  color: white;
}
</style>
