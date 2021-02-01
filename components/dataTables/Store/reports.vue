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
            D Notes
          </th>
          <th
            class="hidden p-3 font-bold text-gray-600 bg-gray-200 border border-gray-300 lg:table-cell"
          >
            Receipt
          </th>

          <th
            class="hidden p-3 font-bold text-gray-600 bg-gray-200 border border-gray-300 lg:table-cell"
          >
            Store Capacity
          </th>
          <th
            class="hidden p-3 font-bold text-gray-600 bg-gray-200 border border-gray-300 lg:table-cell"
          >
            Deliveries
          </th>
          <th
            class="hidden p-3 font-bold text-gray-600 bg-gray-200 border border-gray-300 lg:table-cell"
          >
            Return
          </th>

          <th
            class="hidden p-3 font-bold text-gray-600 bg-gray-200 border border-gray-300 lg:table-cell"
          >
            Payments
          </th>
          <th
            class="hidden p-3 font-bold text-gray-600 bg-gray-200 border border-gray-300 lg:table-cell"
          >
            Incidence
          </th>
        </tr>
      </thead>
      <tbody class="bg-gray-100">
        <!-- Order Row Details -->
        <tr
          v-for="returned in returnedPackage"
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
            <a href="#"> {{ returned.delivery_note }} </a>
          </td>
          <td
            class="relative block w-full p-3 text-center border border-b lg:w-auto lg:table-cell lg:static"
          >
            <span
              class="absolute top-0 left-0 flex items-center h-full px-3 text-xs font-bold uppercase bg-gray-200 text-primary lg:hidden"
              >Category</span
            >
            <a href="#"> {{ returned.receipt }} </a>
          </td>

          <td
            class="relative block w-full p-3 text-center border border-b lg:w-auto text-primary lg:table-cell lg:static"
          >
            <span
              class="absolute top-0 left-0 flex items-center h-full px-3 text-xs font-bold uppercase bg-gray-200 text-primary lg:hidden"
              >To
            </span>
            {{ returned.store_capacity }}
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
              <span class="px-3 py-1 text-xs font-bold bg-green-400 rounded">
                {{ returned.deliveries }}
              </span>
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
              {{ returned.returns }}
            </span>
          </td>

          <td
            class="relative block w-full p-3 text-center border border-b lg:w-auto text-primary lg:table-cell lg:static"
          >
            <span
              class="absolute top-0 left-0 flex items-center h-full px-3 text-xs font-bold uppercase bg-gray-200 text-primary lg:hidden"
              >Status
            </span>
            <span class="px-3 py-1 text-xs font-bold bg-green-400 rounded">
              {{ returned.payments }}
            </span>
          </td>

          <td
            class="relative block w-full p-3 text-center border border-b lg:w-auto text-primary lg:table-cell lg:static"
          >
            <span
              class="absolute top-0 left-0 flex items-center h-full px-3 text-xs font-bold uppercase bg-gray-200 text-primary lg:hidden"
              >Status
            </span>
            <span class="px-3 py-1 text-xs font-bold bg-green-400 rounded">
              {{ returned.incidence }}
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
      returnedPackage: [
        {
          date: "5-Nov",
          order_id: "34101297200",
          delivery_note: "DN1234",
          receipt: "INV-0012",
          destination: "Kisumu",
          store_capacity: "220 sqft",
          deliveries: "320",
          returns: "22",
          packages_log: "500",
          payments: "pending",
          incidence: "resolved",
        },
      ],
    };
  },
};
</script>
