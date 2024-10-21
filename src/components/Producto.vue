<!-- Ejercicio 2: Uso de data bindings y Bootstrap
Crea un componente llamado Producto.vue que muestre el nombre y el precio de un producto.
Además, cambia dinámicamente el color del texto del precio utilizando v-bind y 
usa componentes de Bootstrap, como una lista (list-group). 
Asegúrate de desplegar el proyecto en GitHub. -->

<template>
  <div class="list-group-item">
    <h5 class="mb-1">{{ nombre }}</h5>
    <p :style="{ color }">{{ precio }}</p>
  </div>
</template>

<script>
export default {
  name: "Producto",
  props: ["nombre", "precio", "color"],
};
</script>

<style scoped></style>
