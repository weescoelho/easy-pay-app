<script setup lang="ts">
import Input from "@/components/form/Input.vue";
import EmailIcon from "@/assets/icons/EmailIcon.vue";
import PasswordIcon from "@/assets/icons/PasswordIcon.vue";
import PrimaryButton from "@/components/common/PrimaryButton.vue";
import Circles from "../assets/images/Circles.vue";
</script>

<template>
  <section class="flex flex-row">
    <div class="flex flex-1 flex-col justify-center p-20">
      <h2 class="text-4xl font-bold mb-14">Sign Up</h2>
      <div class="flex flex-col gap-4">
        <Input name="username" label="Username" :icon="EmailIcon" />
        <Input name="password" label="Password" :icon="PasswordIcon" />
      </div>
      <div class="flex items-center justify-center mt-10 flex-col">
        <PrimaryButton label="Sign Up" type="submit" class="w-[400px]" />
        <p class="mt-4 text-sm text-gray-400">
          Do you have an account?
          <a href="#" class="text-purple-500 font-medium hover:text-purple-400"
            >Sign In now</a
          >
        </p>
      </div>
    </div>
    <div
      class="
        bg-purple-500
        lg:w-1/2
        h-screen
        relative
        overflow-hidden
        lg:block
        hidden
      "
    >
      <Circles />
    </div>
  </section>
</template>


