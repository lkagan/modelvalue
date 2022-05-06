<template>
  <CustomTextInput
      v-model="value"
      v-model:lastName="lastName"
  />
  <br />
  First Name: {{ value }}
  <br />
  Last Name: {{ lastName }}


</template>

<script setup>
import CustomTextInput from "@/components/CustomTextInput.vue";
import { ref } from "vue";

const value = ref('');
const lastName = ref('');
</script>