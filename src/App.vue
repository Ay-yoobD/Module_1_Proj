<template>
  <div class="d-flex">
    <NavBar />
    <div class="content flex-grow-1 p-3 position-relative">
      <button class="btn NavButton" type="button" data-bs-toggle="offcanvas" data-bs-target="#offcanvasExample" aria-controls="offcanvasExample">
        ☰ 
      </button>
      <router-view />
    </div>
  </div>
</template>

<script>
import NavBar from "./components/NavBar.vue";

export default {
  components: {
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

.NavButton{
  background-color:#0c2c47;
  color: #97d3cd  ;
  font-size: large;
  position: absolute;
  left: 10px;
  top: 10px;


}

</style>
