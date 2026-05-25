<script setup>
    import { ref } from 'vue'

    const timeNovo = ref('')
    const times = ref([
        'Santos',
        'Gremio',
        'São Paulo',
        'Palmeiras',
        'Corinthians',
        'Flamengo'
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