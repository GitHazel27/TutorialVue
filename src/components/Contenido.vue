<template>
    <section id="contenido" class="contenido">
    <div class="wrapper">
        <div class="contenedor">
            <h2>Tabla de contenido</h2>
            <ul>
                <li><a href="#framework">Framework</a></li>
                <li><a href="#requisitos">Requisitos para programar en Vue</a></li>
                <li><a href="#pasos">Pasos para generar un proyecto</a></li>
                <li><a href="#estructura">Estructura de carpetas o archivos</a></li>
                <li><a href="#componentes">Componentes</a></li>
                <li><a href="#encabezados">Encabezados</a></li>
                <li><a href="#parrafos">Párrafos</a></li>
                <li><a href="#imagenes">Imágenes</a></li>
                <li><a href="#enlaces">Enlaces</a></li>
                <li><a href="#divisiones">Divisiones o contenedores</a></li>
                <li><a href="#listas">Listas</a></li>
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
        margin-top: 10%;
        margin-bottom: 3%;
        font-family:Arial, Helvetica, sans-serif;
        
        text-align: center;
        background-color: #fff;
        border: 2px solid #42B883;
        border-radius: 16px;
        box-shadow: 0 6px 15px rgba(0, 0, 0, 0.15);
        transition: transform 0.3s ease, box-shadow 0.3s ease;
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
    .contenedor a {
        color: rgb(0, 0, 0);
        font-weight: bold;
        font-size: 1.1rem;
        text-decoration: none;
}

html {
    scroll-behavior: smooth;
}

.contenedor-link {
    color: #000;
    text-decoration: none;
    transition: color 0.3s ease;
}

.contenedor a:hover {
    color: #42B883;

}
</style>
