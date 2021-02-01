<template>
  <div>
    <div class="flex mx-auto px-20">
      <div class="w-full">
        <!-- Nav Link -->

        <div class="my-5">
          <nuxt-link
            to="/xstate"
            class="bg-primary text-white px-4 py-1 rounded-md"
            >Add New Package</nuxt-link
          >
        </div>

        <NavRoutes />

        <div class="flex w-full">
          <div class="w-4/6">
            <h1 class="my-3 text-xl">Recent Package Summary</h1>
            <div>
              <table class="w-full my-3 border-collapse shadow-lg">
                <thead>
                  <tr>
                    <th
                      class="hidden p-3 font-bold text-gray-600 bg-gray-200 border border-gray-300 lg:table-cell"
                    >
                      Order#
                    </th>
                    <th
                      class="hidden p-3 font-bold text-gray-600 bg-gray-200 border border-gray-300 lg:table-cell"
                    >
                      Date
                    </th>
                    <th
                      class="hidden p-3 font-bold text-gray-600 bg-gray-200 border border-gray-300 lg:table-cell"
                    >
                      Client
                    </th>
                    <th
                      class="hidden p-3 font-bold text-gray-600 bg-gray-200 border border-gray-300 lg:table-cell"
                    >
                      Category
                    </th>
                    <th
                      class="hidden p-3 font-bold text-gray-600 bg-gray-200 border border-gray-300 lg:table-cell"
                    >
                      Status
                    </th>
                  </tr>
                </thead>
                <tbody class="bg-gray-100">
                  <!-- Order Row Details -->
                  <tr
                    class="flex flex-row flex-wrap mb-10 bg-white lg:hover:bg-gray-100 lg:table-row lg:flex-row lg:flex-no-wrap lg:mb-0"
                  >
                    <td
                      class="relative block w-full p-3 text-center border border-b lg:w-auto lg:table-cell lg:static"
                    >
                      <span
                        class="absolute top-0 left-0 flex items-center h-full px-3 text-xs font-bold uppercase bg-gray-200 text-primary lg:hidden"
                        >Order#</span
                      >
                      <a href="#"> 27101297239 </a>
                    </td>

                    <td
                      class="relative block w-full p-3 text-center border border-b lg:w-auto text-primary lg:table-cell lg:static"
                    >
                      <span
                        class="absolute top-0 left-0 flex items-center h-full px-3 text-xs font-bold uppercase bg-gray-200 text-primary lg:hidden"
                      >
                        Date</span
                      >
                      22-Oct,2020
                    </td>
                    <td
                      class="relative block w-full p-3 text-center text-white border border-b lg:w-auto lg:table-cell lg:static"
                    >
                      <span
                        class="absolute top-0 left-0 flex items-center h-full px-3 text-xs font-bold uppercase bg-gray-200 text-primary lg:hidden"
                        >Delivery</span
                      >

                      <span
                        class="px-3 py-1 text-xs font-bold bg-red-400 rounded"
                        >Aspet Ltd</span
                      >
                    </td>
                    <td
                      class="relative block w-full p-3 text-center border border-b lg:w-auto lg:table-cell lg:static"
                    >
                      <span
                        class="absolute top-0 left-0 flex items-center h-full px-3 text-xs font-bold uppercase bg-gray-200 text-primary lg:hidden"
                        >Category#</span
                      >
                      <a href="#"> Electronics </a>
                    </td>

                    <td
                      class="relative block w-full p-3 text-center border border-b lg:w-auto text-primary lg:table-cell lg:static"
                    >
                      <span
                        class="absolute top-0 left-0 flex items-center h-full px-3 text-xs font-bold uppercase bg-gray-200 text-primary lg:hidden"
                      >
                        Store</span
                      >

                      <a href="">
                        <span
                          class="px-3 py-1 text-xs font-bold bg-green-400 rounded"
                        >
                          On Transit
                        </span>
                      </a>
                    </td>
                  </tr>
                </tbody>
              </table>
            </div>
          </div>
          <div class="flex flex-col p-3">
            <div class="grid grid-cols-1 gap-3">
              <div class="bg-red-200 py-2 flex flex-col items-center p-4">
                <p class="font-bold text-center">Todays Highlights</p>
                <p class="text-sm">Dispatched</p>
                <p class="text-sm">Delivered</p>
                <p class="text-sm">In-store</p>
                <p class="text-sm">Returned</p>
                <p class="text-sm">Uploaded</p>
              </div>

              <div class="bg-red-200 py-2 flex flex-col items-center p-4">
                <p class="font-bold text-center">In-Store to Dispatch Ratio</p>
                <div class="p-3"></div>
              </div>

              <div class="bg-red-200 py-2 flex flex-col items-center p-4">
                <p class="font-bold text-center">Turn Around Time</p>
              </div>

              <div class="bg-red-200 py-2 flex flex-col items-center p-4">
                <p class="font-bold text-center">Increase in volume packages</p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import NavRoutes from "~/components/NavRoutes/packages";
export default {
  components: {
    NavRoutes
  }
};
</script>
