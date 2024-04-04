<template>
    <label :for='labelName'>
        {{ labelName }}
        <select>
            <option disabled value="">Выберите один из вариантов</option>
            <option v-for="item in listItems">
                {{ item }}
            </option>
        </select>
    </label>
</template>

<script setup>
    defineProps(['labelName', 'listItems'])
</script>

<style scoped>
</style>