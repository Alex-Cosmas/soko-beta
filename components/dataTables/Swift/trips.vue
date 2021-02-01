<template>
  <div>
    <table class="w-full my-3 border-collapse shadow-lg">
      <thead>
        <tr>
          <th
            class="hidden p-3 font-bold text-gray-600 bg-gray-200 border border-gray-300 lg:table-cell"
          >
            Dates
          </th>
          <th
            class="hidden p-3 font-bold text-gray-600 bg-gray-200 border border-gray-300 lg:table-cell"
          >
            Code#
          </th>
          <th
            class="hidden p-3 font-bold text-gray-600 bg-gray-200 border border-gray-300 lg:table-cell"
          >
            Client
          </th>
           <th
            class="hidden p-3 font-bold text-gray-600 bg-gray-200 border border-gray-300 lg:table-cell"
          >
            Product
          </th>
          <th
            class="hidden p-3 font-bold text-gray-600 bg-gray-200 border border-gray-300 lg:table-cell"
          >
            Location
          </th>

          <th
            class="hidden p-3 font-bold text-gray-600 bg-gray-200 border border-gray-300 lg:table-cell"
          >
            Route Map
          </th>

           <th
            class="hidden p-3 font-bold text-gray-600 bg-gray-200 border border-gray-300 lg:table-cell"
          >
            ETA
          </th>
          
          <th
            class="hidden p-3 font-bold text-gray-600 bg-gray-200 border border-gray-300 lg:table-cell"
          >
            Driver
          </th>

          <th
            class="hidden p-3 font-bold text-gray-600 bg-gray-200 border border-gray-300 lg:table-cell"
          >
            Delivery Note#
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
          v-for="delivered in deliveredPackageData"
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
            {{ delivered.date }}
          </td>
          <td
            class="relative block w-full p-3 text-center border border-b lg:w-auto lg:table-cell lg:static"
          >
            <span
              class="absolute top-0 left-0 flex items-center h-full px-3 text-xs font-bold uppercase bg-gray-200 text-primary lg:hidden"
              >Order#</span
            >
            <a href="#"> {{ delivered.order_id }} </a>
          </td>
          <td
            class="relative block w-full p-3 text-center border border-b lg:w-auto lg:table-cell lg:static"
          >
            <span
              class="absolute top-0 left-0 flex items-center h-full px-3 text-xs font-bold uppercase bg-gray-200 text-primary lg:hidden"
              >Category</span
            >
            <a href="#"> {{ delivered.category }} </a>
          </td>
          <td
            class="relative block w-full p-3 text-center text-white border border-b lg:w-auto lg:table-cell lg:static"
          >
            <span
              class="absolute top-0 left-0 flex items-center h-full px-3 text-xs font-bold uppercase bg-gray-200 text-primary lg:hidden"
              >Client</span
            >

            <span class="px-3 py-1 text-xs font-bold bg-red-400 rounded">
              {{ delivered.client }}</span
            >
          </td>

          <td
            class="relative block w-full p-3 text-center border border-b lg:w-auto text-primary lg:table-cell lg:static"
          >
            <span
              class="absolute top-0 left-0 flex items-center h-full px-3 text-xs font-bold uppercase bg-gray-200 text-primary lg:hidden"
              >To
            </span>
            {{ delivered.destination }}
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
              <span class="px-3 py-1 text-xs font-bold bg-green-400 rounded">{{
                delivered.assigned_store
              }}</span>
            </a>
          </td>
          <td
            class="relative block w-full p-3 text-center border border-b lg:w-auto text-primary lg:table-cell lg:static"
          >
            <span
              class="absolute top-0 left-0 flex items-center h-full px-3 text-xs font-bold uppercase bg-gray-200 text-primary lg:hidden"
              >Status
            </span>
            <span class="px-3 py-1 text-xs font-bold bg-green-400 rounded">
              {{ delivered.assigned_fleet }}
            </span>
          </td>

          <td
            class="relative block w-full p-3 text-center border border-b lg:w-auto lg:table-cell lg:static"
          >
            <span
              class="absolute top-0 left-0 flex items-center h-full px-3 text-xs font-bold uppercase bg-gray-200 text-primary lg:hidden"
              >Tracking#</span
            >
            <a href="#"> {{ delivered.tracking_id }} </a>
          </td>

          <td
            class="relative block w-full p-3 text-center border border-b lg:w-auto text-primary lg:table-cell lg:static"
          >
            <span
              class="absolute top-0 left-0 flex items-center h-full px-3 text-xs font-bold uppercase bg-gray-200 text-primary lg:hidden"
              >Status
            </span>
            <span class="px-3 py-1 text-xs font-bold bg-green-400 rounded">
              {{ delivered.status }}
            </span>
          </td>
        </tr>
      </tbody>
    </table>
  </div>
</template>



status

<script>
export default {
  data() {
    return {
      returnedPackageData: [
        {
          code: "5-Nov",
          order_id: "34101297200",
          category: "Tapleware",
          client: "Tracko Ltd",
          destination: "Kisumu",
          assigned_store: "Jenga Store",
          assigned_fleet: "Track Ltd",
          tracking_id: "XB-00123",
          status: "Dispatched",
        },
      ],
    };
  },
};
</script>
