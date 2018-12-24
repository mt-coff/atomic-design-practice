<template>
  <div id="app">
    <my-header class="header" />
    <div class="container">
      <side-nav class="side-menu" />
      <router-view class="main-content" />
    </div>
  </div>
</template>

<script>
import MyHeader from "@/components/Organisms/MyHeader.vue";
import SideNav from "@/components/Organisms/SideNav.vue";

export default {
  components: {
    MyHeader,
    SideNav
  }
};
</script>

<style>
body {
  margin: 0;
}
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  min-height: 100vh;
  display: flex;
  flex-direction: column;
}
.container {
  display: flex;
  flex: 1;
}
.side-menu {
  flex: 0 0 15rem;
}
.main-content {
  flex: 1;
  overflow-y: scroll;
  height: 85vh;
}
</style>
