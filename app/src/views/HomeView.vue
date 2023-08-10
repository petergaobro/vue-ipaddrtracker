<template>
  <div class="flex flex-col h-screen max-h-screen">
    <!-- search / results -->
    <div class="flex justify-center relative bg-hero-pattern bg-cover px-4 pt-8 pb-32">
      <!-- search input -->
      <div class="w-full max-w-screen-sm">
        <h1 class="text-white text-center text-3xl pb-4">IP address tracker</h1>
        <div class="flex">
          <input type="text" class="flex-1 py-3 px-2 rounded-tl-md rounded-bl-md focus: outline-none"
            placeholder="please enter here">
          <button class="bg-yellow-500 rounded ml-3 cursor-pointer p-2">search</button>
        </div>
      </div>
      <!-- ip info -->
      <ipInfo />
    </div>

  </div>
</template>

<script>
// @ is an alias to /src
import ipInfo from '@/components/ipInfo.vue';
// import leaflet from "leaflet"
export default {
  name: 'HomeView',
  components: {
    ipInfo
  },
  setup() { },
}
</script>
