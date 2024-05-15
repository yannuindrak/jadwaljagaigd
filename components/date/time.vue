<template>
  <div class="d-flex justify-center">
    <h4 class="text-h6 text-md-h5 text-lg-h4">{{ now }}</h4>
  </div>
</template>

<script setup lang="ts">
import { useNow, useDateFormat } from "@vueuse/core";

const now = useDateFormat(useNow(), "dddd, DD MMMM YYYY HH:mm:ss", {
  locales: "id-ID",
});
</script>
