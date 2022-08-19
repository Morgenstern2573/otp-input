<template>
  <otp 
    :digit-count="4"
    @update:otp="otpValue = $event"
  ></otp>

  <p>The current OTP value is: {{ otpValue }} </p>
</template>

<script setup>
import otp from "./components/OTP.vue";
import { ref } from "vue";

const otpValue = ref('')
</script>
