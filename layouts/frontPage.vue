<template>
  <div class="tracking-wide font-body min-h-screen text-primary bg-green-100">
    <div class="mx-auto px-20">
      <div class="flex">
        <div class="flex ml-auto my-5">
          <nuxt-link to="/client/auth/signUp">
            <p class="px-4 py-1 font-bold border border-gray-200 mr-3">
              Register
            </p>
          </nuxt-link>

          <nuxt-link to="/client/auth/signIn">
            <p
              class="px-4 py-1 font-bold bg-primary text-white text-center rounded-sm"
            >
              Sign In
            </p>
          </nuxt-link>
        </div>
      </div>

      <div class="flex items-center justify-center h-screen">
        <img src="../assets/img/logo-2.svg" alt="" class="h-16" />
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style>
</style>
