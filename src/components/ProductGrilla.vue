<template>
  <div v-if="productos.length === 0">
    <h2>No hay productos en stock</h2>
  </div>
  <div v-else class="grilla">
    <div v-for="producto in productos" :key="producto.id">
        <ProductCard
        :imagen="producto.imagen"
        :categoria="producto.categoria"
        :nombre="producto.nombre"
        :descripcion="producto.descripcion"
        :precio="producto.precio"
        />
    </div>
  </div>
</template>

<script setup>
import ProductCard from './ProductCard.vue';
import { defineProps } from 'vue';

defineProps({
  productos: {
    type: Array,
    default: () => [],
  },
});
</script>

<style scoped>
.grilla {
  display: flex;
  flex-direction: row;
  justify-content: space-around;
  flex-wrap: wrap;
}
</style>
