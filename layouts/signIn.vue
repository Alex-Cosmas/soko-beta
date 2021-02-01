<template>
  <div class="">
    <div class="bg-primary text-white">
      <div class="container mx-auto py-4 flex justify-between">
        <nuxt-link to="/"></nuxt-link>
        <nuxt-link to="">
          <h1>
            <span class="px-3">Dont have an account</span>Click to Register
          </h1>
        </nuxt-link>
      </div>
    </div>
    <div class="mx-auto px-20">
      <div class="min-h-screen flex items-center justify-center">
        <div class="bg-white w-4/5 max-h-full shadow-lg">
          <div class="grid grid-flow-row grid-cols-2 rounded-md">
            <div class="flex flex-col px-8 py-12">
              <div class="flex flex-col mb-3">
                <img src="../assets/img/logo-2.svg" alt="" class="h-10 mb-10" />
              </div>
              <input
                type="text"
                placeholder="Email Address or Mobile Number"
                class="px-4 py-1 border border-gray-200 text-sm w-full mb-1"
              />

              <nuxt-link to="/client/dashboard">
                <button class="bg-primary text-white w-full rounded py-2">
                  Sign In
                </button>
              </nuxt-link>

              <hr class="my-3 text-gray-900" />
              <div>
                <p class="text-sm">Forgot Password?</p>
              </div>

              <hr class="mt-5 text-gray-900 opacity-50" />
              <!-- <div class="flex-col mt-2 leading-tight">
                Sign In using
                <div class="flex">
                  <p class="px-0">Google</p>
                  <p class="px-2">Facebook</p>
                  <p class="px-0">Twitter</p>
                </div>
              </div> -->
            </div>

            <div class="bg-primary text-white px-8 py-12">
              <div>
                <h1 class="text-3xl">Keep your account secure</h1>
                <div>
                  <p
                    class="text-sm leading-tight tracking-wider font-light mt-3"
                  >
                    Shield your Sokplace account with OneAuth app.
                  </p>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>