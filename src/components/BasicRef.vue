<script setup>
import { onMounted,ref } from 'vue'

const myRef = ref('Osayi')
console.log(myRef.value)

onMounted(() => {
    console.log(myRef.value)
    myRef.value.focus()
    myRef.value.value  = 'Osayi'
})
</script>

<!-- template ref -->

<template>

<div>
    <input type="text" placeholder="Enter your Name" ref="myRef" />
</div>
</template>