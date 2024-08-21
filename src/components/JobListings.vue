<script setup>
import JobListing from "./JobListing.vue";
</script>
<template>
  <section class="bg-green-50 px-4 py-10">
    <div class="container-xl lg-container m-auto">
      <h2 class="text-3xl font-bold mb-6 text-green-500 text-center">
        Browse Jobs
      </h2>
      <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
        <JobListing />
        <JobListing />
        <JobListing />
      </div>
    </div>
  </section>
</template>
