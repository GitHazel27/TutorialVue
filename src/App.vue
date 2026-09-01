<script setup lang="ts">
  import {ref} from 'vue'
  import Header from './components/Header.vue';
  import Introduccion from './components/Introduccion.vue';
  import Contenido from './components/Contenido.vue';
  import Encabezados from './components/Encabezados.vue';
  import Parrafos from './components/Parrafos.vue';
  import Imagenes from './components/Imagenes.vue';
  import Enlaces from './components/Enlaces.vue';
  import Divisiones from './components/Divisiones.vue';
</script>

<template>
  <Header></Header>
  <Contenido></Contenido>
  <Introduccion></Introduccion>
  <Encabezados></Encabezados>
  <Parrafos></Parrafos>
  <Imagenes></Imagenes>
  <Enlaces></Enlaces>
  <Divisiones></Divisiones>
</template>

<style scoped>
</style>
