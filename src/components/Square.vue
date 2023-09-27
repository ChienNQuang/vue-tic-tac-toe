<script setup>
    const props = defineProps(['val', 'clickEvent'])
</script>

<template>
    <button class="square" @click="props.clickEvent()">{{props.val}}</button>
</template>