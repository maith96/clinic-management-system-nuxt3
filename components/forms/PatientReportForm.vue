<template>
  <n-form
    ref="formRef"
    size="medium"
  >
    <n-form-item label="Symptoms" path="user.symptoms">
      <n-input :value="formValue.user.symptoms" placeholder="i.e Fever" />
    </n-form-item>
    <n-form-item label="Illness" path="user.illness">
      <n-input :value="formValue.user.illness" placeholder="i.e Malaria" />
    </n-form-item>
    <n-form-item label="Prescription" path="user.prescription">
      <n-input :value="formValue.user.prescription" placeholder="i.e 2pct 2x3" />
    </n-form-item>
    <n-form-item label="DiagnosedBy" path="user.diagnosedBy">
      <n-input :value="formValue.user.diagnosedBy" placeholder="i.e Jane" />
    </n-form-item>
    <n-button>
      Add Report
    </n-button>
  </n-form>
</template>

<script setup lang="ts">
import { FormInst } from 'naive-ui'
const formRef = ref<FormInst | null>(null)
const formValue = ref({
  user: {
    symptoms: '',
    illness: '',
    prescription: '',
    diagnosedBy: ''
  }
})
</script>

<style scoped>

</style>
