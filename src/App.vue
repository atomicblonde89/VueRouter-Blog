<template>
  <div id="app">
    <NavBar />
    <transition name="component-fade" mode="ease-in">
      <router-view />
      <main></main>
    </transition>
    <FooterBar/>
  </div>
</template>

<script>
import NavBar from "./components/NavBar.vue";
import FooterBar from "./components/FooterBar.vue";
export default {
  components: {
    NavBar,
    FooterBar,
  },
};
</script>
<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

* {
  background-image: url("./assets/Manekinekoplaat_1340_c.jpg");
}

nav {
  padding: 30px;
}
a {
  font-weight: bold;
  color: #2c3e50;
}
a.router-link-exact-active {
  color: #42b983;
}
.component-fade-enter-active,
.component-fade-leave-active {
  transition: opacity 1s ease-in;
}
.component-fade-enter, .component-fade-leave-to
/* .component-fade-leave-active below version 2.1.8 */ {
  opacity: 0;
}
</style>
