<template>
  <div>
    <div>123</div>
    <p>Fetched from <pre>/api/mountain</pre>: {{ mountain }}</p>
  </div>
    
</template>

<script setup>
const { data: mountain } = await useFetch('/api/mountain')
</script>
