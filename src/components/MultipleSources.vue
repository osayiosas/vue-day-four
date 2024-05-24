<script setup>
import { ref, watch } from 'vue'

const username = ref('Aseosa')

const counter = ref(0)

watch([username, counter], (newValues, oldValues) => {
  console.log('newValues:', newValues)
  console.log('oldValues:', oldValues)
})
</script> 

<template>
  <h1>Name:{{ username }}</h1>
  <h1>count:{{ counter }}</h1>
  
  <button @click="username = 'Idiaghe'">change name</button>
  <button @click="counter++">Increment counter</button>
</template>