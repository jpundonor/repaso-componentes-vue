<!-- Ejercicio 1: Creación de un componente de tarjeta de perfil con Bootstrap
Crea un componente llamado PerfilUsuario.vue que muestre la información de un usuario, i
ncluyendo su nombre, ocupación y una breve biografía. El diseño debe utilizar las tarjetas (card) de Bootstrap. 
Después, despliega el proyecto en GitHub Pages. -->
<template>
  <div class="card">
    <div class="card-body">
      <h5 class="card-title">{{ nombre }}</h5>
      <span class="card-subtitle mb-2 text-muted">{{ ocupacion }}</span>
      <p class="card-text">{{ biografia }}</p>
    </div>
  </div>
</template>

<script>
export default {
  name: "PerfilUsuario",
  props: ["nombre", "ocupacion", "biografia"],
};
</script>

<style scoped></style>
