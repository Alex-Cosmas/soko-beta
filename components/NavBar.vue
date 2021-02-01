<template>
  <div
    class="mx-auto px-20 bg-green-100 flex justify-between py-2 items-center w-full"
  >
    <div class="w-1/5">
      <nuxt-link to="/client/dashboard">
        <img src="../assets/img/logo-2.svg" alt="" class="h-12" />
      </nuxt-link>
    </div>
    <div class="w-full flex items-center ml-16">
      <MainNav v-if="show" />

      <input
        v-else
        type="text"
        class="px-3 rounded-sm shadow-sm flex flex-grow-1 w-full mx-3"
        placeholder="Search......"
      />
      <p v-on:click="display" class="flex font-bold ml-auto">Search</p>
    </div>
    <div class="flex w-2/5">
      <div class="flex ml-auto">
        <p class="ml-3">Settings</p>
        <div class="h-6 w-6 rounded-full bg-red-900 ml-3"></div>
        <div class="pl-2">
          <nuxt-link to="/">Sign Out</nuxt-link>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import MainNav from "~/components/MainNav/Nav";
export default {
  components: {
    MainNav,
  },
  data() {
    return {
      show: true,
    };
  },
  methods: {
    display() {
      this.show = !this.show;
    },
  },
};
</script>