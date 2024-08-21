<script setup>
import logo from "../assets/img/logo.png";
</script>

<template>
  <nav class="bg-green-700 border-b border-green-500">
    <div class="mx-auto max-w-7xl px-2 sm:px-6 lg:px-8">
      <div class="flex h-20 justify-center items-center">
        <div
          class="flex flex-1 items-center justify-center md:items-stretch md:justify-start"
        >
          <img class="h-10 w-auto" :src="logo" alt="Vue Jobs" />
          <div class="md:ml-auto">
            <ul class="flex space-x-2">
              <li
                class="rounded-md bg-green-900 hover:bg-gray-900 text-white px-3 py-2"
              >
                Home
              </li>
              <li class="rounded-md hover:bg-gray-900 text-white px-3 py-2">
                Jobs
              </li>
              <li class="rounded-md hover:bg-gray-900 text-white px-3 py-2">
                Add Job
              </li>
            </ul>
          </div>
        </div>
      </div>
    </div>
  </nav>
</template>
