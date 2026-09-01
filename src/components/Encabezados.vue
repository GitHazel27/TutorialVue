<template>
    <section id="encabezados" class="encabezados">
        <div class="wrapper">
            <div class="contenedor">
                <h2>Encabezados</h2>
                <p>Definen la jerarquía y estructura de títulos en la página, siendo &lt;h1&gt; el título principal y más importante, descendiendo en relevancia hasta &lt;h6&gt;.</p>

                <button @click="mostrarCodigo = !mostrarCodigo">
                    {{ mostrarCodigo ? 'Ocultar Código' : 'Ver Ejemplo de Código' }}
                </button>

                <pre v-show="mostrarCodigo" class="ejemplo">
                    <code>
                HTML
                &lt;h1&gt;Introducción a Vue.js&lt;/h1&gt;
                &lt;h2&gt;Fundamentos de HTML&lt;/h2&gt;
                &lt;h3&gt;Estructura básica&lt;/h3&gt;
                    </code>
                </pre>
            </div>
        </div>
    </section>
</template>

<script setup lang="ts">
    import {ref} from 'vue'
    const mostrarCodigo = ref(false);
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

    .ejemplo {
        background-color: #1f1d1d;
        padding: 16px;
        border-radius: 30px;
        margin-top: 16px;
        text-align: left;
        font-family: consolas, monospace;
        font-size: 16px;
        color: #fff;
        display: block;
        width: 100%;
        box-sizing: border-box;
        white-space: pre-wrap;
        overflow-x: auto;
    }

    .ejemplo code {
        display: block;
        text-align: left;
        color: #fff;
    }

    button {
        background-color: #42B883;
        color: #fff;
        border: none;
        padding: 10px 20px;
        border-radius: 5px;
        cursor: pointer;
        margin-top: 16px;
    }

    button:hover {
        background-color: #328a67;
    }
</style>