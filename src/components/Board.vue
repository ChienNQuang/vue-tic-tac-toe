<script setup>
import { ref } from "vue";
import Square from "./Square.vue"
const state = ref([])
const clicked = (i) => {
    state[i] = "X"
}
</script>

<template>
    <div class="board-row">
        <Square :val="state[0]" :clickEvent="() => clicked(0)"/>
        <Square :val="state[1]" />
        <Square :val="state[2]" />
    </div>

    <div class="board-row">
        <Square :val="state[3]" />
        <Square :val="state[4]" />
        <Square :val="state[5]" />
    </div>
    <div class="board-row">
        <Square :val="state[6]" />
        <Square :val="state[7]" />
        <Square :val="state[8]" />
    </div>
</template>