<script setup>
import { ref } from 'vue'

const person = ref({
  name: 'John Doe',
  age: 30,
  occupation: 'Developer'
})
</script>

<template>
  <div>
    <h1>{{ person.name }}</h1>
    <p>Age: {{ person.age }}</p>
    <p>Occupation: {{ person.occupation }}</p>
  </div>
</template>
