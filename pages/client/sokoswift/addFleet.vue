<template>
  <div>
    <div class="flex mx-auto px-20">
      <div class="flex flex-col">
        <NavRoutes />
        <div>
          
            <h1 class="my-3 text-xl">Add Fleet - Modal</h1>
            <div>
      
              <p>Code</p>
              <p>Name</p>
              <p>User Name</p>
              <p>Fleet Number</p>
              <p>Location</p>
              <p>Total Fleet</p>
              <p>Email</p>
              <p>Phone</p>
              <p>Business License</p>
              <p>Add Drivert</p>

            </div>

           

          </div>
        </div>
      </div>
    </div>
  </div>
</template>



<script>
import NavRoutes from "~/components/NavRoutes/swift";
import dataTables from "~/components/dataTables/Swift/addFleet";
export default {
  components: {
    NavRoutes,
    dataTables,
  },
};
</script>
