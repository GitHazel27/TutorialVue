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
  import Listas from './components/Listas.vue';
  
</script>

<template>
  <Header></Header>
  <a class="boton-contenido" href="#contenido">
    <svg width="25px" height="25px" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
    <rect width="100" height="100" fill="#42B883"/>
    <path d="M7 14.5L12 9.5L17 14.5" stroke="#000000" stroke-linecap="round" stroke-linejoin="round"/>
    </svg>
  </a>
  <Contenido></Contenido>
  <Introduccion></Introduccion>
  <Encabezados></Encabezados>
  <Parrafos></Parrafos>
  <Imagenes></Imagenes>
  <Enlaces></Enlaces>
  <Divisiones></Divisiones>
  <Listas></Listas>
</template>

<style scoped>
  :global(html), :global(body) {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }

  .boton-contenido {
    position: fixed;
    right: 20px;
    top: 95%;
    transform: translateY(-50%);
    z-index: 1000;
    background-color: #42B883;
    color: white;
    text-decoration: none;
    padding: 12px 18px;
    border-radius: 999px;
    font-weight: bold;
    box-shadow: 0 6px 15px rgba(0, 0, 0, 0.2);
  }

  .boton-contenido:hover {
    background-color: #2f9e6d;
  }

  .boton-contenido:hover rect {
    fill: #2f9e6d;
  }

  .boton-contenido:hover path {
    stroke: #ffffff;
  }
</style>
