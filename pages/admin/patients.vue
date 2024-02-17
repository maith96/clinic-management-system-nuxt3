<script setup lang="ts">

</script>

<template>
  <div class="p-10">
    <n-table>
      <tr>
        <th>Names</th>
        <th>Age</th>
        <th>Gender</th>
        <th>Registered</th>
      </tr>
      <tbody>
        <tr>
          <td>
            <NuxtLink to="/patient-" class="hover:underline hover:text-orange-300">
              Karanja Peter
            </NuxtLink>
          </td>
          <td>34</td>
          <td>Male</td>
          <td>Today 3:00 pm</td>
        </tr>
        <tr>
          <td>
            <NuxtLink to="/" class="hover:underline hover:text-orange-300">
              Jane Mercy
            </NuxtLink>
          </td>
          <td>34</td>
          <td>Male</td>
          <td>Today 3:00 pm</td>
        </tr>
      </tbody>
    </n-table>
    <button class="px-5 py-2 bg-gray-100 hover:bg-blue-400 mt-10">New Patient</button>

    <NewPatientForm />
  </div>
</template>

<style scoped>

</style>
