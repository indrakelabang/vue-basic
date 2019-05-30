<template>
  <div id="app">
    <Header title="VueJs"/>
    <Profile :user="user"/>
  </div>
</template>

<script>
import Header from "./components/Header";
import Profile from "./components/Profile";

export default {
  name: "app",
  components: {
    Header,
    Profile
  },
  data: function() {
    return {
      user: {
        name: "doctor who",
        image: require("./assets/postimage.jpg")
      }
    };
  }
};
</script>

<style>
body {
  margin: 0;
  background-color: #f3f3f3;
}
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
}
</style>
