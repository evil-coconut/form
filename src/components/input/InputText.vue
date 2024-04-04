<template>
    <label :for='labelName'>
        {{ labelName }}
        <input type="text" :id='labelName'/>
    </label>
</template>

<script setup>
    defineProps(['labelName'])
</script>

<style scoped>
</style>