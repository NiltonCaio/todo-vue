<script setup>
    const props = defineProps(['tarefasPendentes', 'verificaPendentes']);
</script>
<template>
    <header class="p-5 mb-4 mt-4 bg-light rounded-3">
        <h1>Minhas tarefas</h1>
        <p v-if="props.verificaPendentes">
            Você possui {{ props.tarefasPendentes }} tarefas pendentes
        </p>
        <span v-else>Não tem tarefas</span>
    </header>
</template>