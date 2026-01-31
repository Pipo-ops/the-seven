<template>
  <div class="basecard">
    <slot name="header" />
    <slot />
    <slot name="footer" />
  </div>
</template>

<script setup>
import { defineProps } from "vue";

defineProps({
  size: {
    type: String,
    default: "md", // sm | md | lg
  },
  hover: {
    type: Boolean,
    default: false,
  },
});
</script>

<style scoped>
.basecard {
  background: #011f35;
  border-radius: 16px;
  box-sizing: border-box;
}
</style>
