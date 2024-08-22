<script setup>
import JobListing from "./JobListing.vue";
import { ref, onMounted } from "vue";
import axios from "axios";

const jobs = ref([]);

onMounted(async () => {
  try {
    const response = await axios.get("http://localhost:5000/jobs");
    jobs.value = response.data;
  } catch (error) {
    console.log("Failed to fetch data", error);
  }
});
</script>
<template>
  <section class="bg-green-50 px-4 py-10">
    <div class="container-xl lg-container m-auto">
      <h2 class="text-3xl font-bold mb-6 text-green-500 text-center">
        Browse Jobs
      </h2>
      <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
        <JobListing v-for="job in jobs" :key="job.id" :job="job" />
      </div>
    </div>
  </section>
</template>
