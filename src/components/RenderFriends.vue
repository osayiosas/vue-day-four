<script setup>

import { ref } from 'vue'

const friends = ref([
    'Joan', 'Amanda', 'John', 'Jane', 'Jack', 'Jill', 'Jenny', 'Jesse', 'Jasmine', 'Jude', 'Jade', 'Jasper', 'idiaghe', 'Jared', 'Jenna', 'odsigbovo', 'Jillian', 'Jax', 'Jazmin', 'Jagger', 'Jazlyn', 'Jovanny', 'Jovany', 'Jovani'
])
</script>

<!-- // Path: src/components/RenderFriends.vue -->

<template>
  <h3 v-for="(friend, i) in friends" :key="i">{{ friends }}</h3>
</template>
