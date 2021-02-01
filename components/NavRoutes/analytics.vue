<template>
  <div>
    <div class="mt-10">
      <ul class="flex py-3">
        <!-- Tab Nav Links -->

        <nuxt-link
          to="/client/analytics/"
          class="px-2 border-b-2 border-gray-200 font-bold"
          >Analytics</nuxt-link
        >
        <nuxt-link to="/client/analytics/turnAround" class="px-2 opacity-30"
          >Turn Around time</nuxt-link
        >
        <nuxt-link
          to="/client/analytics/packageDelivery"
          class="px-2 opacity-30"
          >Package Delivery Rate</nuxt-link
        >
        <nuxt-link to="/client/analytics/fieldRate" class="px-2 opacity-30"
          >Field Rate</nuxt-link
        >
        <nuxt-link to="/client/analytics/returnRate" class="px-2 opacity-30"
          >Return Rate</nuxt-link
        >
      </ul>
    </div>
  </div>
</template>