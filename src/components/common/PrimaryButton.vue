<script setup lang="ts">
defineProps<{
  label: String;
  type?: "submit" | "reset" | "button";
}>();
</script>

<template>
  <button
    class="
      bg-purple-500
      w-full
      rounded-full
      py-2
      text-white
      font-medium
      hover:bg-purple-600
      transition
      easy-in-out
    "
    type="{{type}}"
  >
    {{ label }}
  </button>
</template>
