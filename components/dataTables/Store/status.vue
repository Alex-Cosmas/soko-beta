<template>
  <div>
    <table class="w-full my-3 border-collapse shadow-lg">
      <thead>
        <tr>
          <th
            class="hidden p-3 font-bold text-gray-600 bg-gray-200 border border-gray-300 lg:table-cell"
          >
            Name
          </th>
          <th
            class="hidden p-3 font-bold text-gray-600 bg-gray-200 border border-gray-300 lg:table-cell"
          >
            Order#
          </th>
          <th
            class="hidden p-3 font-bold text-gray-600 bg-gray-200 border border-gray-300 lg:table-cell"
          >
            User
          </th>
          <th
            class="hidden p-3 font-bold text-gray-600 bg-gray-200 border border-gray-300 lg:table-cell"
          >
            Location
          </th>

          <th
            class="hidden p-3 font-bold text-gray-600 bg-gray-200 border border-gray-300 lg:table-cell"
          >
            Industry
          </th>
          <th
            class="hidden p-3 font-bold text-gray-600 bg-gray-200 border border-gray-300 lg:table-cell"
          >
            Email
          </th>
          <th
            class="hidden p-3 font-bold text-gray-600 bg-gray-200 border border-gray-300 lg:table-cell"
          >
            Phone
          </th>

          <th
            class="hidden p-3 font-bold text-gray-600 bg-gray-200 border border-gray-300 lg:table-cell"
          >
            License#
          </th>
          <th
            class="hidden p-3 font-bold text-gray-600 bg-gray-200 border border-gray-300 lg:table-cell"
          >
            Fleet
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
          v-for="status in packageData"
          class="flex flex-row flex-wrap mb-10 bg-white lg:hover:bg-gray-100 lg:table-row lg:flex-row lg:flex-no-wrap lg:mb-0"
        >
          <td
            class="relative block w-full p-3 text-center border border-b lg:w-auto text-primary lg:table-cell lg:static"
          >
            <span
              class="absolute top-0 left-0 flex items-center h-full px-3 text-xs font-bold uppercase bg-gray-200 text-primary lg:hidden"
            >
              Name</span
            >
            {{ status.name }}
          </td>
          <td
            class="relative block w-full p-3 text-center border border-b lg:w-auto lg:table-cell lg:static"
          >
            <span
              class="absolute top-0 left-0 flex items-center h-full px-3 text-xs font-bold uppercase bg-gray-200 text-primary lg:hidden"
              >Order#</span
            >
            <a href="#"> {{ status.order_id }} </a>
          </td>
          <td
            class="relative block w-full p-3 text-center border border-b lg:w-auto lg:table-cell lg:static"
          >
            <span
              class="absolute top-0 left-0 flex items-center h-full px-3 text-xs font-bold uppercase bg-gray-200 text-primary lg:hidden"
              >User</span
            >
            <a href="#"> {{ status.user }} </a>
          </td>
          <td
            class="relative block w-full p-3 text-center text-white border border-b lg:w-auto lg:table-cell lg:static"
          >
            <span
              class="absolute top-0 left-0 flex items-center h-full px-3 text-xs font-bold uppercase bg-gray-200 text-primary lg:hidden"
              >Industry</span
            >

            <span class="px-3 py-1 text-xs font-bold bg-red-400 rounded">
              {{ status.location }}</span
            >
          </td>

          <td
            class="relative block w-full p-3 text-center border border-b lg:w-auto text-primary lg:table-cell lg:static"
          >
            <span
              class="absolute top-0 left-0 flex items-center h-full px-3 text-xs font-bold uppercase bg-gray-200 text-primary lg:hidden"
              >Location
            </span>
            {{ status.industry }}
          </td>
          <td
            class="relative block w-full p-3 text-center border border-b lg:w-auto text-primary lg:table-cell lg:static"
          >
            <span
              class="absolute top-0 left-0 flex items-center h-full px-3 text-xs font-bold uppercase bg-gray-200 text-primary lg:hidden"
            >
              Email</span
            >

            <a href="">
              <span
                class="truncate px-3 py-1 text-xs font-bold bg-green-400 rounded"
                >{{ status.email }}</span
              >
            </a>
          </td>
          <td
            class="relative block w-full p-3 text-center border border-b lg:w-auto text-primary lg:table-cell lg:static"
          >
            <span
              class="absolute top-0 left-0 flex items-center h-full px-3 text-xs font-bold uppercase bg-gray-200 text-primary lg:hidden"
              >Phone No
            </span>
            {{ status.phone_no }}
          </td>

          <td
            class="relative block w-full p-3 text-center border border-b lg:w-auto lg:table-cell lg:static"
          >
            <span
              class="absolute top-0 left-0 flex items-center h-full px-3 text-xs font-bold uppercase bg-gray-200 text-primary lg:hidden"
              >License#</span
            >
            <a href="#"> {{ status.license_id }} </a>
          </td>
          <td
            class="relative block w-full p-3 text-center border border-b lg:w-auto lg:table-cell lg:static"
          >
            <span
              class="absolute top-0 left-0 flex items-center h-full px-3 text-xs font-bold uppercase bg-gray-200 text-primary lg:hidden"
              >fleet#</span
            >
            <a href="#"> {{ status.fleet }} </a>
          </td>

          <td
            class="relative block w-full p-3 text-center border border-b lg:w-auto text-primary lg:table-cell lg:static"
          >
            <span
              class="absolute top-0 left-0 flex items-center h-full px-3 text-xs font-bold uppercase bg-gray-200 text-primary lg:hidden"
              >Status
            </span>
            <span class="px-3 py-1 text-xs font-bold bg-green-400 rounded">
              {{ status.status }}
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
      packageData: [
        {
          name: "Sema Ltd",
          order_id: "34101297200",
          user: "John M",
          industry: "Tracko Ltd",
          location: "Kisumu",
          email: "jengastore@email.com",
          phone_no: "Track Ltd",
          license_id: "XB-00123",
          fleet: "1234",
          status: "Dispatched",
        },
      ],
    };
  },
};
</script>
