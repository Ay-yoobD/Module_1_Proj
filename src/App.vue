<template>
  <div class="d-flex"> <!-- Bootstrap's flex container -->
    <NavBar />
    <div class="content flex-grow-1 p-3">
      <router-view />
    </div>
  </div>
</template>

<script>
  import NavBar from "./components/NavBar.vue";

  export default {
    components:{
      NavBar
    }
    
  }
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

</style>
