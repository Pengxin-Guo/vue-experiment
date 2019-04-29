<template>
  <div id="app">
    <myheader />
    <div id="main">
      <sidebar />
      <myarticle />
    </div>
    <myfooter />
  </div>
</template>

<script>
export default {
  components: {
    myheader: () => import("./views/Header"),
    sidebar: () => import("./views/Sidebar"),
    myfooter: () => import("./views/Footer"),
    myarticle: () => import("./views/Article")
  }
};
</script>

<style>
#main {
  margin: 5px 0px;
  border: 1px solid red;
}
</style>
