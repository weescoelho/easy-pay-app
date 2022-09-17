<script setup lang="ts">
import PrimaryButton from "./common/PrimaryButton.vue";
import Blueball from "../assets/images/Blueball.vue";
import PurpleStar from "../assets/images/PurpleStar.vue";
import Purpleball from "../assets/images/Purpleball.vue";
import Orangeball from "../assets/images/Orangeball.vue";
</script>

<template>
  <section class="flex items-center mt-40 gap-5 relative">
    <Blueball class="absolute top-0 right-[600px]" />
    <PurpleStar class="absolute top-8 lg:left-[500px] right-2" />
    <Purpleball class="absolute bottom-0 hidden lg:block" />
    <Orangeball class="absolute right-0 bottom-3 hidden lg:block" />
    <div>
      <h1 class="text-7xl max-w-[670px] font-bold mb-5">
        Payments made easy on Easy Pay
      </h1>
      <p class="mb-8 text-lg text-gray-500">
        A platform for accepting payment, making payments and paying bills
      </p>
      <div class="flex gap-5 max-w-[430px]">
        <PrimaryButton type="button" label="Get Started" />
        <PrimaryButton type="button" label="Join our Community" />
      </div>
    </div>
    <div class="hidden lg:block">
      <img src="../assets/images/Cashout.png" alt="EasyPay cashout image" />
    </div>
  </section>
</template>