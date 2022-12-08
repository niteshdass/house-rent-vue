<script setup>
defineProps({
  id: {
    type: String,
    default: "message",
  },
  rows: {
    type: Number,
    default: 8,
  },
  placeholder: {
    type: String,
    default: "",
  },
  labelClass: {
    type: String,
    default: "",
  },
});
</script>
<template>
  <div class="input-group">
    <label :for="id" :class="labelClass"><slot /></label>
    <textarea
      name="message"
      class="form-control"
      :id="id"
      :placeholder="placeholder"
      :rows="rows"
      style="border: 1px solid #d2d6da; padding: 10px;"
    />
  </div>
</template>
