<template>
    <label :for='labelName'>
        {{ labelName }}
        <input type="number" :id='labelName'/>
    </label>
</template>

<script setup>
    defineProps(['labelName'])
</script>

<style scoped>
</style>