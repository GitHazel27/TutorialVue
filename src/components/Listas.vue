<template>
    <section id="listas" class="listas">
        <div class="wrapper">
            <div class="contenedor">
                <h2>Listas</h2>
                <p>Elementos utilizados para mostrar información en formato de lista, ya sea ordenada o no ordenada.</p>

                <div class="tabs">
                    <button
                        :class="{ activo: moduloActivo === 'ol' }"
                        @click="moduloActivo = 'ol'"
                    >
                        Listas Ordenadas
                    </button>
                    <button
                        :class="{ activo: moduloActivo === 'ul' }"
                        @click="moduloActivo = 'ul'"
                    >
                        Listas No Ordenadas
                    </button>
                </div>

                <section v-if="moduloActivo === 'ol'">
                    <h2>Listas Ordenadas &lt;ol&gt; y &lt;li&gt;</h2>
                    <p class="descripcion">Presentan una secuencia de elementos con orden numérico o alfabético específico, ideal para pasos de instalación o guías secuenciales.</p>

                    <button @click="mostrarCodigo = !mostrarCodigo">
                        {{ mostrarCodigo ? 'Ocultar Código' : 'Ver Ejemplo de Código' }}
                        </button>

                    <pre v-show="mostrarCodigo" class="ejemplo">
                        <code>
        HTML
                
        &lt;ol&gt;
            &lt;li&gt;Instalar dependencias con npm install&lt;/li&gt;
            &lt;li&gt;Ejecutar npm run dev en la terminal&lt;/li&gt;
            &lt;li&gt;Abrir el enlace local en el navegador&lt;/li&gt;
        &lt;/ol&gt;
                        </code>
                    </pre>
                </section>

                <section v-else-if="moduloActivo === 'ul'">
                    <h2>Listas No Ordenadas &lt;ul&gt; y &lt;li&gt;</h2>
                    <p class="descripcion">Muestran un conjunto de elementos relacionados donde el orden no es relevante; cada elemento de la lista se define con &lt;li&gt; y se representa con viñetas.</p>

                    <button @click="mostrarCodigo = !mostrarCodigo">
                        {{ mostrarCodigo ? 'Ocultar Código' : 'Ver Ejemplo de Código' }}
                        </button>

                    <pre v-show="mostrarCodigo" class="ejemplo">
                        <code>
        HTML
                
        &lt;ul&gt;
            &lt;li&gt;Visual Studio Code&lt;/li&gt;
            &lt;li&gt;Node.js&lt;/li&gt;
            &lt;li&gt;Vite&lt;/li&gt;
        &lt;/ul&gt;
                        </code>
                    </pre>
                </section>

                
            </div>
        </div>
    </section>
</template>

<script setup lang="ts">
    import {ref} from 'vue'
    const moduloActivo = ref();
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

    .tabs {
        display: flex;
        gap: 12px;
        flex-wrap: wrap;
        justify-content: center;
        margin: 16px 0;
    }

    .tabs button {
        margin: 0;
        background-color: #d9f5eb;
        color: #1f3d2e;
        border: 1px solid #42B883;
    }

    .tabs button:hover {
        background-color: #42B883;
        color: #fff;
    }

    .tabs button.activo {
        background-color: #42B883;
        color: #fff;
        box-shadow: 0 2px 8px rgba(66, 184, 131, 0.35);
    }

    .descripcion {
        text-align: justify;
        margin-top: 8px;
        margin-bottom: 16px;
    }
</style>