<template>
  <div>
    <div class="mt-10">
      <ul class="flex py-3">
        <!-- Tab Nav Links -->

        <nuxt-link to="/client/sokostore/" class="">Status</nuxt-link>
        <nuxt-link to="/client/sokostore/mapview" class="px-2 opacity-30"
          >Map View</nuxt-link
        >
        <nuxt-link to="/client/sokostore/packagelist" class="px-2 opacity-30"
          >Package</nuxt-link
        >

        <nuxt-link to="/client/sokostore/addStore" class="px-2 opacity-30"
          >Add Store</nuxt-link
        >
        <nuxt-link to="/client/sokostore/reports" class="px-2 opacity-30"
          >Reports</nuxt-link
        >
        <nuxt-link to="/client/sokostore/returned" class="px-2 opacity-30"
          >Returned</nuxt-link
        >
      </ul>
    </div>
  </div>
</template>