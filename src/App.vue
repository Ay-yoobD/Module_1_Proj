<template>
  <div class="d-flex">
    <!-- Show NavBar only if NOT on login page -->
    <NavBar v-if="showNavbar" />

    <div class="content flex-grow-1 p-3">
      <router-view />
    </div>
  </div>
</template>

<script>
import NavBar from "./components/NavBar.vue";
import { computed } from "vue";
import { useRoute } from "vue-router";

export default {
  components: {
    NavBar,
  },
  setup() {
    const route = useRoute();

    // Hide NavBar on login page (route name 'login')
    const showNavbar = computed(() => route.name !== "login");

    return {
      showNavbar,
    };
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
  min-height: 100vh;
}

/* Optional: Make sure content fills space when sidebar is hidden */
.content {
  width: 100%;
}
</style>
