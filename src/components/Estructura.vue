<template>
    <section id="estructura" class="estructura">
    <div class="wrapper">
        <div class="contenedor">
            <h2>Estructura de carpetas o archivos</h2>
            <ul>
            <li><b>node_modules/:</b> Contiene todas las librerías y dependencias instaladas esenciales para el funcionamiento del proyecto.</li>
            <li><b>public/:</b> Directorio para recursos estáticos del proyecto.</li>  
            <li><b>src/:</b> Carpeta principal de código fuente que contiene los componentes, estilos y lógica de la aplicación:  
                <ul>
                    <li><b>src/App.vue:</b> Componente raíz principal de la aplicación.</li>
                    <li><b>src/components/:</b> Carpeta destinada a almacenar componentes individuales (como HelloWorld.vue).</li>
                    <li><b>src/main.js (o main.ts):</b> Archivo de entrada de JavaScript/TypeScript que monta la aplicación de Vue.</li>
                    <li><b>src/style.css:</b> Archivo de hojas de estilo globales.</li>
                </ul>
            </li>
            <li><b>index.html:</b> Página principal de entrada del proyecto web donde se monta la aplicación.</li>
            <li><b>package.json:</b> Archivo de configuración que define los metadatos del proyecto, scripts de ejecución (dev, build, preview) y la lista de dependencias (vue, @vitejs/plugin-vue).</li>
            <li><b>package-lock.json:</b> Registro exacto de las versiones y dependencias instaladas.</li>
            <li><b>vite.config.ts / vite.config.js:</b> Archivo de configuración del empaquetador Vite.</li>
            <li><b>.gitignore:</b> Lista de archivos y directorios excluidos del control de versiones de Git.</li>
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
        padding-left: 1.5rem;
        width: 100%;
        list-style-position: outside;
        text-align: left;
        box-sizing: border-box;
    }

    .contenedor li {
        line-height: 1.6;
        margin-left: 0.5rem;
    }

    .contenedor ul ul {
        margin-top: 0.5rem;
        padding-left: 1.5rem;
    }
</style>