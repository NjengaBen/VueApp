<script setup>
import { RouterLink } from "vue-router";
</script>
<template>
  <div class="bg-white rounded-xl shadow-md relative">
    <div class="p-4">
      <div class="mb-6">
        <div class="text-gray-600 my-2">Full Time</div>
        <h3 class="text-xl font-bold">Senior Vue Developer</h3>
      </div>
      <div class="mb-5">
        We are seeking a talented Front-End Developer to join our team in
        Boston, MA. The ideal candidate will have strong skills in HTML, CSS,
        and JavaScript...
      </div>
      <h3 class="text-green-500 mb-2">$70-$80K / Year</h3>
      <div class="border border-gray-100 mb-3"></div>
      <div class="flex flex-col lg:flex-row justify-between mb-4">
        <div class="text-orange-700 mb-3">
          <div class="pi pi-map-marker text-lg"></div>
          Boston, MA
        </div>
        <RouterLink
          to="/jobs/:id"
          class="h-[36px] bg-green-500 hover:bg-green-600 rounded-lg px-4 py-2 text-white text-center text-sm"
          >Read More</RouterLink
        >
      </div>
    </div>
  </div>
</template>
