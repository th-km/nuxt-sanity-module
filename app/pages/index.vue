<script setup lang="ts">
const query = groq`*[]`
const { data } = await useSanityQuery(query)
</script>

<template>
  <div>
    <pre>{{ JSON.stringify(data, null, 2) }}</pre>
  </div>
</template>
