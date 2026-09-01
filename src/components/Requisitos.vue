<template>
    <section id="requisitos" class="requisitos">
    <div class="wrapper">
        <div class="contenedor">
            <h2>Requisitos para programar en Vue</h2>
            <p>Para trabajar con Vue.js, se necesitan algunos requisitos básicos:</p>
            <ul>
                <li>Node.js: Versión ^20.19.0 o >=22.12.0 (puede utilizarse la versión integrada en Laragon).</li>
                <li>Editor de código: Visual Studio Code con las siguientes extensiones recomendadas:</li>
                <ul>
                    <li>Vue - oficial</li>
                    <li>Auto Close Tag</li>
                    <li>Prettier - Code formatter</li>
                    <li>Peacock</li>
                    <li>Alpine IntelliSense</li> 
                </ul>
                <li>Control de versiones: Cuenta en GitHub.</li>
            </ul>
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

    .contenedor ul {
        display: flex;
        flex-direction: column;
        align-items: flex-start;
        justify-content: flex-start;
        gap: 0.5rem;
        margin: 0;
        padding: 0 2rem;
        width: 100%;
        list-style-position: inside;
    }
</style>