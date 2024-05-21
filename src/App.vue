<template>
  <div>
    <Card v-for="product in products" :key="product.ID" :product="product" />
  </div>
</template>

<script setup>
import { ref } from 'vue';
import Card from './components/Card.vue'; 

const products = ref([
  {
    ID: 1,
    Prenume: "Maria",
    Nume: "Anders",
    City: "Berlin",
    "Postal Code": 12209,
    Country: "Germany",
  },
  {
    ID: 2,
    Prenume: "Ana",
    Nume: "Trujillo",
    City: "México D.F.",
    "Postal Code": 15021,
    Country: "Mexico",
  },
]);
</script>

<style scoped>
</style>
