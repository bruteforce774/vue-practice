<script setup>
import { ref } from 'vue'


defineProps(['msg'])

const count = ref(0);
</script>

<template>
    <div>
        <h1>{{ msg }}</h1>

        <div>
            <input type="range" min="1" max="100" v-bind:value="count"></input>
            <button type="button" @click="count++">count is {{ count }}</button>
        </div>
    </div>
</template>