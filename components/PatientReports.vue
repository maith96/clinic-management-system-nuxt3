<script setup lang="ts">

</script>

<template>
  <div>
    <n-table>
      <legend>Reports</legend>
      <tr>
        <th>Id</th>
        <th>Symptoms</th>
        <th>Illness</th>
        <th>Prescription</th>
        <th>Diagnosed by</th>
        <th>Date</th>
      </tr>
      <tbody>
        <tr>
          <td>34e-uy6-89i</td>
          <td>
            <ul>
              <li>Headache</li>
              <li>Fever</li>
            </ul>
          </td>
          <td>Malaria</td>
          <td>
            <ul>
              <li>2pct 3x2</li>
            </ul>
          </td>
          <td>Dr. Lavender</td>
          <td>16th December 2023</td>
        </tr>
      </tbody>
      <NuxtLink to="/patient/2/new-report">
        New Report
      </NuxtLink>
    </n-table>
  </div>
</template>

<style scoped>

</style>
