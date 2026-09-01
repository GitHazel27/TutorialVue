<template>
    <section id="pasos" class="pasos">
    <div class="wrapper">
        <div class="contenedor">
            <h2>Pasos para generar un proyecto</h2>
            <ol>
                <li>Comprobar la versión instalada de Node en la terminal con node -v.</li>
                <li>Abrir la terminal y ubicarse en el directorio de trabajo deseado (por ejemplo, laragon/www).</li>
                <li>Ejecutar el comando de inicialización: npm create vite@latest.</li>
                <li>Asignar el nombre del proyecto (ejemplo: projectvite1).</li>
                <li>Seleccionar el framework: Vue.</li>
                <li>Seleccionar la variante deseada (JavaScript o TypeScript).</li>
                <li>Ingresar a la carpeta del proyecto e instalar las dependencias con npm install (o npm i).</li>
                <li>Iniciar el servidor local de desarrollo ejecutando npm run dev.</li>
            </ol>
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

    .contenedor ol {
        display: flex;
        flex-direction: column;
        align-items: flex-start;
        justify-content: flex-start;
        gap: 0.5rem;
        margin: 2% 0;
        padding: 0 2rem 0 1rem;
        width: 100%;
        box-sizing: border-box;
    }
</style>