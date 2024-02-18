<template>
  <n-form
      ref="formRef"
      size="medium"
  >
    <n-form-item label="DoctorId" path="user.doctorId">
      <n-input :value="formValue.user.doctorId" placeholder="i.e 23-45t-6yh7" />
    </n-form-item>
    <n-form-item label="PatientId" path="user.patientId">
      <n-input :value="formValue.user.patientId" placeholder="i.e 23-45t-6yh7" />
    </n-form-item>
    <n-form-item label="dateTime" path="user.dateTime">
      <n-input :value="formValue.user.dateTime" placeholder="i.e 4/5/2024" />
    </n-form-item>

    <n-button>
      Schedule Appointment
    </n-button>
  </n-form>
</template>

<script setup lang="ts">
import { FormInst } from 'naive-ui'
const formRef = ref<FormInst | null>(null)
const formValue = ref({
  user: {
    doctorId: '',
    patientId: '',
    dateTime: ''
  }
})
</script>

<style scoped>

</style>
