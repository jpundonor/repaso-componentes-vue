<!-- Ejercicio 3: Formulario interactivo con Bootstrap y v-model
Crea un componente llamado FormularioUsuario.vue que tenga dos campos de entrada 
donde el usuario pueda ingresar su nombre y su edad, utilizando v-model. Muestra los valores ingresados en tiempo real.
Usa el sistema de formularios de Bootstrap y despliega el proyecto en GitHub Pages. -->
<template>
  <form class="form">
    <div class="form-group">
      <label for="nombre">Nombre:</label>
      <input type="text" class="form-control" v-model="nombre" />
    </div>
    <div class="form-group">
      <label for="edad">Edad:</label>
      <input type="number" class="form-control" v-model="edad" />
    </div>
  </form>
  <div class="alert alert-info" role="alert">
    Nombre: {{ nombre }} Edad: {{ edad }}
  </div>
</template>

<script>
export default {
  name: "FormularioUsuario",
  data() {
    return {
      nombre: "",
      edad: "",
    };
  },
};
</script>

<style scoped></style>
