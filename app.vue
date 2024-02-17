<template>
  <NuxtLayout>
    <NuxtPage />
  </NuxtLayout>
</template>

<script setup lang="ts">
const examples = ref<any | null>(null)

async function add () {
  const example = await $fetch('/api/example/1', {
    method: 'put',
    body: { details: 'det', description: 'description' }
  })
  console.log('examples: ', example)
  examples.value = await $fetch('/api/example', {})
  console.log(examples)
}


</script>
