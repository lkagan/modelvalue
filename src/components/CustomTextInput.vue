<template>
  <label for="">First Name</label>
  <input
      type="text"
      placeholder="Input"
      :value="modelValue"
      @input="$emit('update:modelValue', $event.target.value)"
  />
  <br />
  <label for="">Last Name</label>
  <input
      type="text"
      placeholder="Input"
      :value="lastName"
      @input="$emit('update:lastName', $event.target.value)"
  />
</template>

<script setup>

defineProps({
  modelValue: String,
  lastName: String
});

</script>

<style>
</style>
