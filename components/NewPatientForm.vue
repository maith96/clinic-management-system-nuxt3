<template>
  <n-form
    ref="formRef"
    size="medium"
  >
    <n-form-item label="firstName" path="user.firstName">
      <n-input :value="formValue.user.firstName" placeholder="i.e Jane" />
    </n-form-item>

    <n-form-item label="lastName" path="user.lastName">
      <n-input :value="formValue.user.lastName" placeholder="i.e Mercy" />
    </n-form-item>
    <n-form-item label="middleName" path="user.middleName">
      <n-input :value="formValue.user.middleName" placeholder="i.e Kelvin" />
    </n-form-item>

    <n-form-item label="contact" path="user.contact">
      <n-input :value="formValue.user.contact" placeholder="i.e +254756354278" />
    </n-form-item>

    <n-form-item label="Age" path="user.age">
      <n-input :value="formValue.user.age" placeholder="i.e 32" />
    </n-form-item>

    <n-form-item label="Gender" path="user.gender">
      <n-input :value="formValue.user.gender" placeholder="i.e Male" />
    </n-form-item>

    <n-form-item label="Height (metres)" path="user.height">
      <n-input :value="formValue.user.height" placeholder="i.e 34 m" />
    </n-form-item>

    <n-button>
      Register new patient
    </n-button>
  </n-form>
</template>


<script setup lang="ts">
import { FormInst } from 'naive-ui'
const formRef = ref<FormInst | null>(null)
const formValue = ref({
  user: {
    firstName: '',
    lastName: '',
    middleName: '',
    contact: '',
    age: '',
    gender: '',
    height: ''
  }
})
</script>


<style scoped>

</style>
