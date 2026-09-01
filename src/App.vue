<script setup lang="ts">
  import {ref} from 'vue'
  import Body from './components/Body.vue';
  import Header from './components/Header.vue';
import Introduccion from './components/Introduccion.vue';
import Contenido from './components/Contenido.vue';
import Encabezados from './components/Encabezados.vue';
import Parrafos from './components/Parrafos.vue';
</script>

<template>
  <Header></Header>
  <Contenido></Contenido>
  <Introduccion></Introduccion>
  <Encabezados></Encabezados>
  <Parrafos></Parrafos>
  
</template>

<style scoped>
</style>
