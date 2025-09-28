<script setup>
import { ref } from 'vue'


defineProps(['msg'])

const count = ref(9)
</script>

<template>
    <div>
        <h1 v-show="count<10">Mindre enn 10</h1>

        <div>
            <input type="range" min="1" max="100" v-model="count"></input>
            <button type="button" @click="count++">count is {{ count }}</button>
        </div>
    </div>
</template>