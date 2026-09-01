<template>
    <section id="framework" class="framework">
    <div class="wrapper">
        <div class="contenedor">
            <h2>Framework</h2>
            <p>Consiste en una estructura y conjunto de herramientas estandarizadas de código abierto para el desarrollo frontend.  Permite construir aplicaciones web dinámicas e interactivas de forma declarativa y reactiva.  Organiza el código mediante una arquitectura basada en componentes reutilizables que integran plantilla, lógica y estilos.  </p>
        </div>
    </div>
    </section>
</template>

<script setup lang="ts">
</script>

<style scoped>

    .wrapper{
    width: 100%;
    height: auto;
    padding: 24px;
    box-sizing: border-box;
    display: flex;
    justify-content: center;
    align-items: center;
    background-color: #35495E;
    border: 1px solid #42B883;
    }
    .contenedor{
    width: 70%;
    height: auto;
    padding: 24px;
    box-sizing: border-box;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    margin-top: 3%;
    margin-bottom: 3%;
    font-family:Arial, Helvetica, sans-serif;
    
    text-align: center;
    background-color: #fff;
    border: 2px solid #42B883;
    border-radius: 16px;
    box-shadow: 0 6px 15px rgba(0, 0, 0, 0.15);
    transition: transform 0.3s ease, box-shadow 0.3s ease;
    }

    .contenedor > p{
        text-align: justify;
    }
</style>