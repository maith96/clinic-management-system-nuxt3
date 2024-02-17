<script setup lang="ts">
const options = [{ label: 'Sign Out', key: 'Sign Out' }]
function handleSelect () {

}
</script>

<template>
  <div class="p-10 flex justify-between">
    <NuxtLink to="/" class="mr-10">Clinic Management System</NuxtLink>

    <n-dropdown trigger="hover" :options="options" @select="handleSelect" :show-arrow="true">
      <span>Dr. Johane David</span>
    </n-dropdown>
  </div>

</template>

<style scoped>

</style>
