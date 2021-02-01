<template>
  <div>
    <div class="mt-10">
      <ul class="flex py-3">
        <!-- Tab Nav Links -->

        <nuxt-link to="/client/clients" class="">All Clients</nuxt-link>

        <nuxt-link to="/client/clients/accounts" class="px-2 opacity-30"
          >Accounts</nuxt-link
        >

        <nuxt-link to="/client/clients/orders" class="px-2 opacity-30"
          >Orders</nuxt-link
        >

        <nuxt-link to="/client/clients/payments" class="px-2 opacity-30"
          >Payments</nuxt-link
        >

        <nuxt-link to="/client/clients/reports" class="px-2 opacity-30"
          >Reports</nuxt-link
        >
      </ul>
    </div>
  </div>
</template>