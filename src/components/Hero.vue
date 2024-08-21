<script setup>
import { defineProps } from "vue";

defineProps({
  title: {
    type: String,
    default: "Become a Vue Dev",
  },
  description: {
    type: String,
    default: "Find the vue job that fits your skills and needs",
  },
});
</script>
<template>
  <section class="bg-green-700 py-20 mb-4">
    <div
      class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 flex flex-col items-center"
    >
      <div class="text-center">
        <h2 class="text-4xl text-white font-extrabold sm:text-5xl md:text-6xl">
          {{ title }}
        </h2>
        <p class="my-4 text-xl text-white">{{ description }}</p>
      </div>
    </div>
  </section>
</template>
