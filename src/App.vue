<template>
<NavBar></NavBar>
  <div>
    <ProductGrilla :productos="objetos" />
  </div>
  <FooterC></FooterC>
</template>

<script setup>
import NavBar from "./components/NavBar.vue";
import ProductGrilla from "./components/ProductGrilla.vue";
//JSON//////////////////////////////////////////
import objetos from "../src/assets/productos.json";
import FooterC from "./components/FooterC.vue";

</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
