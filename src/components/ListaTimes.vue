<script setup>
    import { ref } from 'vue'

    const timeNovo = ref('')
    const times = ref([
        'Santos',
        'Gremio',
        'São Paulo'
    ])

    function adicionar(){
        times.value.push(timeNovo.value)
        timeNovo.value = ''
    }
</script>

<template>
    <h2>Lista de Times</h2>
    <input type="text" v-model="timeNovo">
    <button @click="adicionar">Adicionar Time</button>
    <ul>
        <li v-for="time in times" :key="time">{{ time }}</li>
    </ul>
</template>

<style scoped>
    h2 {
        color: #333;
    }

    input {
        padding: 5px;
        margin-right: 10px;
    }

    button {
        padding: 5px 10px;
        background-color: #4CAF50;
        color: white;
        border: none;
        border-radius: 5px;
        cursor: pointer;
    }

    button:hover {
        background-color: #45a049;
    }

    ul {
        list-style-type: none;
        padding: 0;
    }

    li {
        background-color: #f0f0f0;
        margin-bottom: 5px;
        padding: 10px;
        border-radius: 5px;
    }

</style>