<template>
  <div>
    <ProductGrilla :productos="objetos" />
  </div>
</template>

<script setup>
import ProductGrilla from "./components/ProductGrilla.vue";

//JSON//////////////////////////////////////////
import objetos from "../src/assets/productos.json";
//JSON//////////////////////////////////////////
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
