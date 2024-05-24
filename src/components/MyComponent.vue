<script setup>
import { ref } from "vue";

//when using the <script setup>
// - its private by default
// - A parent reference a child wont be able to access anthing.

// - first we have to expose all the properties and methods
// - we want to be able to access from the parent component

//- use use (defineExpose) to expose our data to the parent component  to use.
const count = ref(10)
const increment = () => count.value++
const decrement = () => count.value--


defineExpose({
    count,
    increment,
    decrement
})

</script>

<template>
    <h1>{{ count }}</h1>
    <button @click="increment">Increment</button>
    <button @click="decrement">Decrement</button>
</template>