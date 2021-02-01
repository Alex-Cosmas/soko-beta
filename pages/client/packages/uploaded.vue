<template>
  <div>
    <div class="flex mx-auto px-20">
      <div class="flex flex-col">
        <NavRoutes />
        <div>
          
                       <h1 class="my-3 text-xl">Uploaded Packages</h1>

            <table class="w-full my-3 border-collapse shadow-lg">
              <thead>
                <tr>
                  <th
                    class="hidden p-3 font-bold text-gray-600 bg-gray-200 border border-gray-300 lg:table-cell"
                  >
                    Date
                  </th>
                  <th
                    class="hidden p-3 font-bold text-gray-600 bg-gray-200 border border-gray-300 lg:table-cell"
                  >
                    Order#
                  </th>
                  <th
                    class="hidden p-3 font-bold text-gray-600 bg-gray-200 border border-gray-300 lg:table-cell"
                  >
                    Category
                  </th>
                  <th
                    class="hidden p-3 font-bold text-gray-600 bg-gray-200 border border-gray-300 lg:table-cell"
                  >
                    Client
                  </th>

                  <th
                    class="hidden p-3 font-bold text-gray-600 bg-gray-200 border border-gray-300 lg:table-cell"
                  >
                    Destination
                  </th>
                  <th
                    class="hidden p-3 font-bold text-gray-600 bg-gray-200 border border-gray-300 lg:table-cell"
                  >
                    Assigned Store
                  </th>
                  <th
                    class="hidden p-3 font-bold text-gray-600 bg-gray-200 border border-gray-300 lg:table-cell"
                  >
                    Assigned Fleet
                  </th>

                  <th
                    class="hidden p-3 font-bold text-gray-600 bg-gray-200 border border-gray-300 lg:table-cell"
                  >
                    Tracking#
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
                    class="relative block w-full p-3 text-center border border-b lg:w-auto text-primary lg:table-cell lg:static"
                  >
                    <span
                      class="absolute top-0 left-0 flex items-center h-full px-3 text-xs font-bold uppercase bg-gray-200 text-primary lg:hidden"
                    >
                      Dates</span
                    >
                    22-Oct,2020
                  </td>
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
                    class="relative block w-full p-3 text-center border border-b lg:w-auto lg:table-cell lg:static"
                  >
                    <span
                      class="absolute top-0 left-0 flex items-center h-full px-3 text-xs font-bold uppercase bg-gray-200 text-primary lg:hidden"
                      >Category</span
                    >
                    <a href="#"> Electronics </a>
                  </td>
                  <td
                    class="relative block w-full p-3 text-center text-white border border-b lg:w-auto lg:table-cell lg:static"
                  >
                    <span
                      class="absolute top-0 left-0 flex items-center h-full px-3 text-xs font-bold uppercase bg-gray-200 text-primary lg:hidden"
                      >Client</span
                    >

                    <span class="px-3 py-1 text-xs font-bold bg-red-400 rounded"
                      >Apset Ltd</span
                    >
                  </td>

                  <td
                    class="relative block w-full p-3 text-center border border-b lg:w-auto text-primary lg:table-cell lg:static"
                  >
                    <span
                      class="absolute top-0 left-0 flex items-center h-full px-3 text-xs font-bold uppercase bg-gray-200 text-primary lg:hidden"
                      >To
                    </span>
                    Kisumu
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
                        >Assign Store</span
                      >
                    </a>
                  </td>
                  <td
                    class="relative block w-full p-3 text-center border border-b lg:w-auto text-primary lg:table-cell lg:static"
                  >
                    <span
                      class="absolute top-0 left-0 flex items-center h-full px-3 text-xs font-bold uppercase bg-gray-200 text-primary lg:hidden"
                      >Status
                    </span>
                    <span
                      class="px-3 py-1 text-xs font-bold bg-green-400 rounded"
                    >
                      Assign Store
                    </span>
                  </td>

                  <td
                    class="relative block w-full p-3 text-center border border-b lg:w-auto lg:table-cell lg:static"
                  >
                    <span
                      class="absolute top-0 left-0 flex items-center h-full px-3 text-xs font-bold uppercase bg-gray-200 text-primary lg:hidden"
                      >Tracking#</span
                    >
                    <a href="#"> 27101297239 </a>
                  </td>

                  <td
                    class="relative block w-full p-3 text-center border border-b lg:w-auto lg:table-cell lg:static"
                  >
                    <span
                      class="absolute top-0 left-0 flex items-center h-full px-3 text-xs font-bold uppercase bg-gray-200 text-primary lg:hidden"
                      >Tracking#</span
                    >

                    

                    <div class="dropdown inline-block relative">
                      <button
                        class="bg-gray-300 text-gray-700 font-semibold py-2 px-4 rounded inline-flex items-center"
                      >
                        <span class="mr-1">Pending</span>
                        <svg
                          class="fill-current h-4 w-4"
                          xmlns="http://www.w3.org/2000/svg"
                          viewBox="0 0 20 20"
                        >
                          <path
                            d="M9.293 12.95l.707.707L15.657 8l-1.414-1.414L10 10.828 5.757 6.586 4.343 8z"
                          />
                        </svg>
                      </button>
                      <ul
                        class="dropdown-menu absolute hidden text-gray-700 pt-1"
                      >
                        <li class="">
                          <a
                            class="rounded-t bg-gray-200 hover:bg-gray-400 py-2 px-4 block whitespace-no-wrap"
                            href="#"
                            >One</a
                          >
                        </li>
                        <li class="">
                          <a
                            class="bg-gray-200 hover:bg-gray-400 py-2 px-4 block whitespace-no-wrap"
                            href="#"
                            >Two</a
                          >
                        </li>
                        <li class="">
                          <a
                            class="rounded-b bg-gray-200 hover:bg-gray-400 py-2 px-4 block whitespace-no-wrap"
                            href="#"
                            >Three is the magic number</a
                          >
                        </li>
                      </ul>
                    </div>
                  </td>
                </tr>
              </tbody>
            </table>
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
    NavRoutes,
  },
};
</script>

   
