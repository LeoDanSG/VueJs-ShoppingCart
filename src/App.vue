<script setup>
//Importando funcion para crear referencias reactivas
import { ref } from 'vue'
//Creando una referencia de tipo string
const header = ref('App Lista de compras');
const shoppingIcon = ref('material-icons shopping-cart-icon');
</script>

//Pegamos el const de shoppingIcon para mostrar la figura
<template>
  <h1> <i v-bind:class="shoppingIcon">local_mall</i> {{ header }}</h1>
</template>

<style scoped>
.shopping-cart-icon {
  font-size: 2rem;
}
</style>
