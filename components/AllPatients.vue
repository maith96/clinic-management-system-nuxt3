<script setup lang="ts">

</script>

<template>
  <div>
    <n-table class="">
      <legend>Patients</legend>
      <tr>
        <th>Id</th>
        <th>Patient</th>
        <th>Doctor</th>
        <th>Time</th>
      </tr>
      <tbody>
        <tr>
          <td>werf-ity-oepw</td>
          <td>Mr. Juma</td>
          <td>Dr. Mercy</td>
          <td>24th February 2024</td>
        </tr>
      </tbody>
    </n-table>
    <NuxtLink to="/auth/register/patient">New Patient</NuxtLink>
  </div>
</template>

<style scoped>

</style>
