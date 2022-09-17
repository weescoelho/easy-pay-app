<template>
  <div class="flex flex-col gap-2">
    <label for="{{name}}" class="font-medium text-xl">{{ label }}</label>
    <div class="relative">
      <input
        type="password"
        name="{{name}}"
        class="
          border border-gray-400
          h-10
          rounded-full
          w-full
          px-10
          outline-indigo-500
        "
      />
      <component :is="icon" class="absolute bottom-3 right-4 cursor-pointer" />
    </div>
  </div>
</template>

<script setup lang="ts">
defineProps<{
  label: String;
  name: String;
  icon: any;
}>();
</script>