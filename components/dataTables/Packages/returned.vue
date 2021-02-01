<template>
  <div>
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
          v-for="returned in returnedPackageData"
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
            {{ returned.date }}
          </td>
          <td
            class="relative block w-full p-3 text-center border border-b lg:w-auto lg:table-cell lg:static"
          >
            <span
              class="absolute top-0 left-0 flex items-center h-full px-3 text-xs font-bold uppercase bg-gray-200 text-primary lg:hidden"
              >Order#</span
            >
            <a href="#"> {{ returned.order_id }} </a>
          </td>
          <td
            class="relative block w-full p-3 text-center border border-b lg:w-auto lg:table-cell lg:static"
          >
            <span
              class="absolute top-0 left-0 flex items-center h-full px-3 text-xs font-bold uppercase bg-gray-200 text-primary lg:hidden"
              >Category</span
            >
            <a href="#"> {{ returned.category }} </a>
          </td>
          <td
            class="relative block w-full p-3 text-center text-white border border-b lg:w-auto lg:table-cell lg:static"
          >
            <span
              class="absolute top-0 left-0 flex items-center h-full px-3 text-xs font-bold uppercase bg-gray-200 text-primary lg:hidden"
              >Client</span
            >

            <span class="px-3 py-1 text-xs font-bold bg-red-400 rounded">
              {{ returned.client }}</span
            >
          </td>

          <td
            class="relative block w-full p-3 text-center border border-b lg:w-auto text-primary lg:table-cell lg:static"
          >
            <span
              class="absolute top-0 left-0 flex items-center h-full px-3 text-xs font-bold uppercase bg-gray-200 text-primary lg:hidden"
              >To
            </span>
            {{ returned.destination }}
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
                returned.assigned_store
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
              {{ returned.assigned_fleet }}
            </span>
          </td>

          <td
            class="relative block w-full p-3 text-center border border-b lg:w-auto lg:table-cell lg:static"
          >
            <span
              class="absolute top-0 left-0 flex items-center h-full px-3 text-xs font-bold uppercase bg-gray-200 text-primary lg:hidden"
              >Tracking#</span
            >
            <a href="#"> {{ returned.tracking_id }} </a>
          </td>

          <td
            class="relative block w-full p-3 text-center border border-b lg:w-auto text-primary lg:table-cell lg:static"
          >
            <span
              class="absolute top-0 left-0 flex items-center h-full px-3 text-xs font-bold uppercase bg-gray-200 text-primary lg:hidden"
              >Status
            </span>
            <span class="px-3 py-1 text-xs font-bold bg-green-400 rounded">
              {{ returned.status }}
            </span>
          </td>
        </tr>
      </tbody>
    </table>
  </div>
</template>


<script>
export default {
  data() {
    return {
      returnedPackageData: [
        {
          date: "5-Nov",
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

   