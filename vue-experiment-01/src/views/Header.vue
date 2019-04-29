<template>
  <div>
    <ul>
      <li>
        <a class="active" href="#">Home</a>
      </li>
      <li>
        <a href="#">News</a>
      </li>
      <li>
        <a href="#">Contact</a>
      </li>
      <li>
        <a href="#">About</a>
      </li>
      <li class="right">
        <a href="#">Logout</a>
      </li>
    </ul>
  </div>
</template>

<style scoped>
div {
  padding: 5px;
  border: 1px solid red;
  margin: 5px 10px;
}
/* 基于后代/子选择器，减少类的数量，降低与HTML的耦合 */
ul {
  display: flex;
  list-style-type: none;
  margin: 0;
  padding: 0;
  background-color: #333;
}
a {
  display: block; /* 变为block级，填充高宽 */
  color: white;
  text-align: center;
  padding: 14px 16px;
  text-decoration: none;
}
.active {
  background-color: #4caf50;
}
/* 上导航鼠标悬停样式 */
a:hover {
  background-color: #111;
}
/* 导航中右对齐内容样式，li元素样式 */
.right {
  margin-left: auto;
}
</style>
