<template>
  <div id='app' class='container-fluid h-100'>
    <div class='row h-100'>
      <div class='col-md-2 sidebar'>
        <SideBar />
      </div>
      <div class='col-md-10 main'>
        <router-view />
      </div>
    </div>
  </div>
</template>

<script>
import SideBar from "./components/shared/SideBar.vue";
export default {
  name: "App",
  components: {
    SideBar,
  },
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
.sidebar {
  position: fixed!important;
  top: 0;
  left: 0;
  height: 100vh;
  background-color: #656565;
}
.main {
  background-color: #3e3e3e;
  color: #ffffff;
  margin-left: 16.666667%;
}
body {
  height: 100%;
}
html {
  height: 100%;
}
</style>
