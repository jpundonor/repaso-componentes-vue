<template>
  <PerfilUsuario
    nombre="Choripan con Pebre"
    ocupacion="Desarrollador"
    biografia="Lorem ipsum dolor sit amet, consectetur adipiscing elit."
  />
  <FormularioUsuario />

  <ListaProductos :productos="productos" />
</template>

<script>
import FormularioUsuario from "./components/FormularioUsuario.vue";
import ListaProductos from "./components/ListaProductos.vue";
import PerfilUsuario from "./components/PerfilUsuario.vue";

export default {
  components: {
    FormularioUsuario,
    ListaProductos,
    PerfilUsuario,
  },
  data() {
    return {
      productos: [
        { nombre: "Choripan", precio: "$1000", color: "red" },
        { nombre: "Empanada", precio: "$2000", color: "green" },
        { nombre: "Terremoto", precio: "$1500", color: "purple" },
      ],
    };
  },
};
</script>

<style scoped></style>
