<template>
  <div>
    <div class="mt-10">
      <ul class="flex py-3">
        <!-- Tab Nav Links -->

        <nuxt-link to="/client/packages/" class="">All Packages</nuxt-link>
        <nuxt-link to="/client/packages/uploaded" class="px-2 opacity-30"
          >Uploaded</nuxt-link
        >
        <nuxt-link to="/client/packages/onTransit" class="px-2 opacity-30"
          >On Transit</nuxt-link
        >
        <nuxt-link to="/client/packages/received" class="px-2 opacity-30"
          >Received</nuxt-link
        >
        <nuxt-link to="/client/packages/dispatched" class="px-2 opacity-30"
          >Dispatched</nuxt-link
        >
        <nuxt-link to="/client/packages/delivered" class="px-2 opacity-30"
          >Delivered</nuxt-link
        >
        <nuxt-link to="/client/packages/returned" class="px-2 opacity-30"
          >Returned</nuxt-link
        >
      </ul>
    </div>
  </div>
</template>