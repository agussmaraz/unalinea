<template>
  <div>
    <Navbar @sidenavtoggle="displaySidenav = !displaySidenav" />
    <TheSidenav :v-show="displaySidenav" :show="displaySidenav" @close="displaySidenav = false" />
    <Nuxt />
  </div>
</template>
<script>
import Navbar from "@/components/Navigation/NavBar.vue";
import TheSidenav from "@/components/Navigation/TheSidenav";
export default {
  components: {
    Navbar,
    TheSidenav
  },
  data() {
    return {
      displaySidenav: false
    };
  }
};
</script>

<style>
html {
  font-family: "Open Sans", sans-serif;
}
</style>
