<template>
  <div id="app">
    <sidebar id="sidebar" />
    <router-view id="main" />
  </div>
</template>

<script>
export default {
  components: { sidebar: () => import("@/views/Sidebar.vue") }
};
</script>

<style>
#sidebar {
  vertical-align: top;
  margin: 10px;
  display: inline-block;
  border: 1px solid red;
  width: 200px;
}
#main {
  vertical-align: top;
  margin: 10px;
  display: inline-block;
  border: 1px solid red;
  width: calc(100% - 250px);
}
</style>
