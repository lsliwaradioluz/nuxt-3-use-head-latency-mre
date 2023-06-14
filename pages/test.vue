<template>
  <div>
    <h1 :class="`heading-${id}`">Test</h1>
    <p>Test page</p>
  </div>
</template>

<script setup>
const id = '12345';

useHead({
  style: [{
    id,
    textContent: `
      .heading-${id} {
        color: red;
      }
    `
  }]
})
</script>