<template>
    <section id="componentes" class="componentes">
    <div class="wrapper">
        <div class="contenedor">
            <h2>Componentes</h2>
            <b>Qué es:</b> Es una unidad de código modular e independiente (Single-File Component o .vue) dividida internamente en tres bloques estructurales:  
            <ul>
            <li><b>&lt;template&gt;:</b> Define la estructura HTML y directivas de la vista.</li>
            <li><b>&lt;script setup&gt;:</b> Contiene la lógica en JavaScript/TypeScript y el manejo de reactividad.</li>
            <li><b>&lt;style&gt;:</b> Contiene los estilos y reglas CSS del elemento.</li>
            </ul>
            <b>Para qué sirve:</b> Sirve para encapsular y reutilizar bloques funcionales de la interfaz de usuario, recibir parámetros (props), emitir eventos y mantener variables reactivas aisladas y mantenibles dentro de la aplicación. 
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

    .contenedor {
        text-align: justify;
    }

    .contenedor > p{
        text-align: justify;
    }

    .contenedor ul {
        width: 100%;
        margin: 0.5rem 0 1rem;
        padding-left: 1.5rem;
        text-align: justify;
    }

    .contenedor li {
        margin-bottom: 0.4rem;
    }
</style>