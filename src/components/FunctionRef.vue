<script setup>

const myRefFunc = (el) => {
    console.log(el.textContent);
    el.textContent = "this is new value";
    el.style.color = "red";

}

</script>

<!-- function Ref  -->

<template>
    <h1 :ref="myRefFunc">this intial value</h1>
</template>