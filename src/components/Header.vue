<template>
    <header>
        <nav>
            <h1>Bienvenidos al tutorial de Vue</h1>
        </nav>
    </header>
</template>

<script setup lang="ts">
</script>

<style scoped>
header{
    font-family: sans-serif;
    font-weight: bold;
    text-align: center;
    position: sticky;
    top: 0;
    z-index: 1000;
    background-color: #fff;
    box-shadow: 0 4px 15px rgba(0, 0, 0, 0.2);
}
header {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    z-index: 1000;
}

main {
    padding-top: 80px;
}
nav{
    max-width: 100%;
    width: 100%;
    background-color: #F8FAFC;
    border-radius: 10px;
    width: 100%;
    height: 60px;
    display: block;
    padding: 10px 14px;
    /*box-shadow: 0 8px 25px rgb(4, 4, 4);*/
}

nav h1{
    color:#42B883;
    text-decoration: none;
}

</style>