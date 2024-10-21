<!-- Ejercicio 4: Lista de productos con props y Bootstrap
Crea dos componentes: uno llamado ListaProductos.vue que reciba una lista de productos mediante props, 
y otro componente Producto.vue que se encargue de renderizar cada producto individualmente. 
Usa las tarjetas (card) de Bootstrap para mostrar cada producto. 
Asegúrate de desplegar el proyecto en GitHub Pages. -->

<template>
  <div v-for="producto in productos">
    <Producto
      :nombre="producto.nombre"
      :precio="producto.precio"
      :color="producto.color"
    />
  </div>
</template>

<script>
import Producto from "./Producto.vue";

export default {
  name: "ListaProductos",
  props: {
    productos: Array,
  },
  components: {
    Producto,
  },
};
</script>

<style scoped></style>
