<script setup>
    defineProps({
        times: String,
        comp: String
    })

    
</script>

<template>
    <section>
        <h2>Time</h2>
        <p><strong>Nome: </strong> {{ times }} </p>
        <p><strong>Competição: </strong> {{ comp }} </p>
    </section>
</template>

<style scoped>
    section{
        background-color: #f0f0f0;
        padding: 20px;
        border-radius: 5px;
        box-shadow: 0 5px 5px rgba(0, 0, 0, 0.3);
    }
</style>