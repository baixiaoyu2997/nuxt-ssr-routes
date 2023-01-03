<template>
  <div>
    <div>123</div>
    <p>Fetched from <pre>/api/mountain</pre>: {{ mountain }}</p>
    <button @click="onClick">Fetch</button>
  </div>
    
</template>

<script setup>
const { data: mountain } = await useFetch('/api/mountain')
const onClick=async ()=>{
  const { data: test } = await useFetch('/api/test')
}
</script>
